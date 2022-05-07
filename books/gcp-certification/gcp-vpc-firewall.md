---
title: "ファイアウォール"
---
# ファイアウォールとは
ファイアウォールとは、コンピュータやネットワークとの通信を設定したポリシーに従って許可または拒否するセキュリティ機能のこと。  
例えばクラウドの外からアクセスしてくるユーザの端末とCE間のネットワーク通信を制御する。  
![](https://storage.googleapis.com/zenn-user-upload/00f7405786bf-20220507.png =400x)

# ファイアーウォールルールの設定要素^[<https://cloud.google.com/vpc/docs/firewalls?hl=ja>]
ユーザが定義したファイアウォールルールを利用して、Google Cloudサービスへのアクセスを制御。  
Google Cloudではデフォルトで外部IPアドレスのTCPポート25（SMTP）を宛先とする通信は許可されない。
![](https://storage.googleapis.com/zenn-user-upload/087d17fda316-20220507.png =600x)