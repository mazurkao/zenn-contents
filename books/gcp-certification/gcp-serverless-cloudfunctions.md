---
title: "Cloud Functioins"
---
# Cloud Functioinsとは^[<https://cloud.google.com/functions/docs/concepts/events-triggers?hl=ja#functions_parameters-python>]
Cloud Functioinsは、HTTPリクエストや各種サービスのイベントをトリガーに、関数を実行するサーバレスサービスです。  
関数単位での実行になるため、シンプルなシステムの構築に向いています。  
イベントと関数を組み合わせることで様々な処理を行える反面、特定のプログラミング言語しかサポートしておらず、利用する上で制約が多いことが特徴です。
![](https://storage.googleapis.com/zenn-user-upload/69ab9408c4e0-20220507.png =600x)  

## イベント
イベントは、クラウド環境内で発生するもので、対策を講じる必要があります。たとえば、データベースでのデータの変更、ストレージ システムへのファイルの追加、新しい仮想マシン インスタンスの作成などがイベントとして扱われます。 現在、Cloud Functions では次のプロバイダのイベントがサポートされています。
- HTTP
- Cloud Storage
- Cloud Pub/Sub
- Cloud Firestore
- Firebase（Realtime Database、Storage、アナリティクス、Auth）
- Cloud Logging - シンクを作成して、ログエントリを Pub/Sub トピックに転送します。その後、この関数をトリガーできます。

## トリガー
イベントへのレスポンスはトリガーにより行われます。トリガーは、特定のイベントや一連のイベントに関心があることを示すものにもなります。 関数をトリガーにバインドすると、イベントをキャプチャして処理できます。
