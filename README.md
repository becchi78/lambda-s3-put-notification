# lambda-s3-put-notification

S3 のバケットに拡張子.txt のファイルを PUT すると Lambda が実行され、"lambda invoked!"と表示する Cloudformation のテンプレートです。

# 実行方法
```
aws cloudformation deploy \
    --template-file template.yaml \
    --capabilities CAPABILITY_NAMED_IAM \ --stack-name lambda-s3-put-notification \
    --s3-bucket cfn-template-lambda-s3-put-notification \
```