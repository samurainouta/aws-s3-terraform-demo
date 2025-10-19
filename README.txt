# Terraformで作るAWS S3バケットポートフォリオ

## 概要
このプロジェクトは、Terraformを使用してAWS上にS3バケットを自動作成するデモです。
PowerShellでTerraformを実行し、AWS CLIで認証情報を設定して作成しました。

## 技術スタック
- AWS CLI
- Terraform
- PowerShell

## デモ手順
1. AWS CLIで認証情報を設定
```bash
aws configure

## Terraformコードのポイント
- `provider "aws"` : AWSの認証情報とリージョンを指定
- `resource "aws_s3_bucket"` : S3バケットを作成
- `bucket` 名前はグローバルで一意にする必要あり
- `acl = "private"` でバケットを非公開に設定

## 学んだこと
Infrastructure as Code(IaC)の基本概念
Terraformの初期化、適用、削除の流れ
AWS CLIによる認証設定
S3バケットの作成・確認・削除操作
GitHubでポートフォリオとして管理する方法
