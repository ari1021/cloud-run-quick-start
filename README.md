# cloud-run-quick-start

- プロジェクトの切り替え
```
gcloud config set project <your-project-id>
```
- コンテナイメージのビルド
```
gcloud builds submit --tag gcr.io/<your-project-id>/<your-image-name>
```
- コンテナイメージのデプロイ
```
gcloud run deploy --image gcr.io/<your-project-id>/<your-image-name> --platform managed
```