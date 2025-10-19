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
