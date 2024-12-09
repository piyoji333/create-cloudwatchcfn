# create-cloudwatchcfn

## 構成

Cloudfront - S3 - API Gateway - Lambda


構築方法

1.S3バケットを作成

2.cloudfrontを作成して先ほどのバケットをオリジンにする

SSL設定などは適宜設定


3.Lambda関数の作成

3-1.作業フォルダ作成
3-2.function.zipからlambda関数をデプロイ
    タイムアウト値などは適宜修正


4.API Gatewayを作成

HTTP API
Routes POST
Integrations 作成したLambda関数
CORS すべて"*"

変更後デプロイを行う
エンドポイントをコピーしてindex.htmlに追加する

