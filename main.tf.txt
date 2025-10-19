# main.tf

provider "aws" {
  region = "ap-northeast-1"  # 東京リージョン
}

# S3バケットを作成
resource "aws_s3_bucket" "my_bucket" {
  bucket = "my-portfolio-s3-bucket-kei-20251019"
  acl    = "private"

  tags = {
    Name        = "TerraformDemo"
    Environment = "Dev"
  }
}
