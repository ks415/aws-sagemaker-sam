# 概要

AWS サービスを使用して Segment Anything Model (SAM)をデプロイし，画像認識用のサーバーレス API エンドポイントを作成．

## セットアップ手順

1. **リポジトリのクローン**

```bash
git clone https://github.com/yourusername/aws-sagemaker-sam.git
```

2. **インフラストラクチャのデプロイ**

```bash
cd aws-sagemaker-sam/terraform
terraform init
terraform plan
terraform apply
```

3. **API のテスト**

```bash
curl -X POST https://{api-endpoint}/v1/predict \
    -H "Content-Type: application/json" \
    -d '{"image_url": "https://example.com/image.jpg"}'
```
