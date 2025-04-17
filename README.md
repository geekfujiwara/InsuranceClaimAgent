# InsuranceClaimAgent 事故対応エージェント
破損した車の画像やユーザーに状況をヒアリングし事故対応を円滑に行うエージェントです。

![image](https://github.com/user-attachments/assets/202a0776-80ea-4782-b323-a44c9db0157a)



https://github.com/user-attachments/assets/ca218d51-ff3a-43c0-9ce9-f7a1dabe106f


### インポート方法
[最新のソリューション](https://github.com/geekfujiwara/ProcurementOrderCheck/releases/tag/InsuranceClaimAgent)をダウンロードします。

[Power Apps ポータル](https://make.powerapps.com/)にアクセスします。

ファイルをアップロードしてインポートします。

![image](https://github.com/user-attachments/assets/6553eb87-9d77-40fc-9709-ae8e6079cc34)

接続が作成されるまで待ち、完了したらインポートします。

![image](https://github.com/user-attachments/assets/16374618-dbeb-4e11-b214-0a696bbf4f0e)

>[!Note]
>もしこのような警告が表示されても大丈夫です。これはCopilot Studio のライセンスが不足しているという警告であり、インポート自体に問題があるわけではありません。 Copilot Studio のトライアルを行うこともできますのでこのまま進めます。
>
>![image](https://github.com/user-attachments/assets/0768bc6d-13c4-4e23-8a2d-9351852353f5)

ソリューションにアクセスします。

![image](https://github.com/user-attachments/assets/333bc56d-5c06-4b77-9b3a-540910a0be37)

すべてのカスタマイズを公開します。

![image](https://github.com/user-attachments/assets/c27ccb31-6b8f-4996-8c2f-6a69794c5235)

これでソリューションのインポートが完了しました。

## 利用方法

ソリューションには保険申請を起票するエージェントと、保険申請を管理する Power Apps モデル駆動型アプリが含まれています。

事故対応エージェント (保険申請を起票するエージェント)

![image](https://github.com/user-attachments/assets/2ca9da4f-94ea-4fd4-95de-e6a0969b940c)

保険申請管理 (保険申請を管理する Power Apps モデル駆動型アプリ)
![image](https://github.com/user-attachments/assets/a03a801e-dd2a-4324-9b4f-a03fb0d204d0)


まずは事故対応エージェントにて、用件を選択します。

![image](https://github.com/user-attachments/assets/3f5eae43-e18e-4266-b593-793614c3c66e)

損傷した車の画像を送付します。例えばこれらの画像を利用してください。

![車の損傷画像 (3)](https://github.com/user-attachments/assets/868da423-c7b8-472b-b3da-2dc050f6fdb0)
![車の損傷画像 (2)](https://github.com/user-attachments/assets/9637c5ec-bfa5-443e-97d1-6de2c8340b52)
![車の損傷画像 (1)](https://github.com/user-attachments/assets/fb32ac67-9641-46dd-8250-c1d1c45e23f3)

これは車が損傷したというトピックの上で動作しています。

![image](https://github.com/user-attachments/assets/cdca6b26-80d5-4cae-b238-240e984de023)


## カスタマイズ

### ナレッジを変更する場合:

参照させたいナレッジがある場合自由に変更することができます。自社の保証規約について含めることができます。

>[!Note]
>保証規約が様々なパターンがある場合は、トピックにて選択させて特定の契約内容から回答させることを推奨します。

![image](https://github.com/user-attachments/assets/13067884-30af-49e2-ad30-a82a798e0ea0)

### 公開
エージェントはエージェントの作成者の権限で動作するように設定されていますので、外部に公開される際は十分注意してください。
外部への公開はチャネルから行うことができます。外部チャネルでの[添付ファイルの有効化はBot Framework](https://learn.microsoft.com/ja-jp/azure/bot-service/rest-api/bot-framework-rest-connector-add-media-attachments?view=azure-bot-service-4.0) で行う必要があります。

以上

