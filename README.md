## 概要

デプロイしたアカウント上で最小キャパシティが0.5ではないAurora Serverlessクラスタが作成された場合最小キャパシティを0.5に変更する仕組み。

詳しくは以下の記事もご参照ください。  
https://dev.classmethod.jp/articles/aurora-serverless-capacity-auto-decrease/

## ビルド・デプロイ

以下のコマンドを実行します。

```
 sam build && sam deploy --parameter-overrides NotificationReceiverAddress={{your mail address}}
```

初回デプロイ時はAmazon SNS利用のための確認が上記で指定したアドレスに来るので承認確認が必要です。

