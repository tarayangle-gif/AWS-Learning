# AWS-Learning
AWS　and Linux　Learning　records
# AWS Learning

## About

AWSやLinuxの学習記録です。

## Environment

- AWS EC2
- Amazon Linux
- nginx

## Learning Record

### 2026-07-14

- VPC作成
- Public Subnet構築
- EC2起動
- Elastic IP設定
- nginxインストール
- Web公開成功


## 2026-07-15

### Today

- NAT Gatewayについて学習
- Private Subnet作成

### Learned

NAT GatewayはPrivate Subnetから外へ通信するための出口。

### Trouble

EC2からSSH接続できなかった。

### Solution

# TerraformでAWS環境を構築

## 作成したリソース

- VPC
- Public Subnet
- Internet Gateway
- Route Table
- Security Group
- EC2

## 発生したエラー①

InvalidKeyPair.NotFound

### 原因

AWSに存在しないキーペアを指定していた。

### 対応

既存のキーペア名へ変更。

---

## 発生したエラー②

Free Tier対象外インスタンス

### 原因

対象外のインスタンスタイプだった。

### 対応

Free Tier対象へ変更。

---

## 学んだこと

Terraformはコードを書くだけではなく、
エラー内容を読み解いて修正することが重要。

Security Groupの22番ポート設定を確認した。
