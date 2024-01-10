# command

## CloudFormationファイル出力

```shell
% aws cloudformation package \
  --template-file template.yml \
  --s3-bucket sam-app-hands-on-yosnak-1 \
  --output-template-file packaged-template.yml
```

## リソースのデプロイ

```shell
% aws cloudformation deploy \
  --template-file ./packaged-template.yml \
  --stack-name sam-app-hands-on-yosnak-1 \
  --capabilities CAPABILITY_IAM
```
