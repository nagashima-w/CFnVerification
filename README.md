# CFnVerification
## なにこれ

- 検証用のコンテナをCFnでCI組んで自動デプロイしたい

## コマンド備忘録

- テンプレートの構成を確認するとき

```bash
aws cloudformation validate-template --template-body file://verification-template.yml
```

- スタックを作成するとき

```bash
aws cloudformation create-stack --template-body file://verification-template.yml --stack-name cfn-verification
```

- スタックを確認するとき

```bash
aws cloudformation describe-stack --stack-name cfn-verification
```

- スタックを削除するとき

```bash
aws cloudformation delete-stack --stack-name cfn-verification
```