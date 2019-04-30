AWS Tutorials

# Tutorials


## Code Deploy

https://docs.aws.amazon.com/ja_jp/codedeploy/latest/userguide/welcome.html

CodeDeployは、Amazon EC2インスタンスやオンプレミスインスタンス、サーバーレス Lambda 関数、
またはAmazon ECSサービスに対するアプリケーションのデプロイを自動化するデプロイメントサービス。

以下のようなアプリケーションコンテンツをデプロイできる

- コード
- サーバーレス AWS Lambda 関数
- ウェブファイルおよび設定ファイル
- 実行可能ファイル
- packages
- スクリプト
- マルチメディアファイル

### デプロイ操作手順

1. インスタンスの作成/IAMロールの作成
2. アプリケーションの作成
3. デプロイ設定/グループの作成
4. リビジョンの作成

Deploy使用方法

* [CodeDeploy エージェントの使用](https://docs.aws.amazon.com/ja_jp/codedeploy/latest/userguide/codedeploy-agent.html)
* [インスタンスの使用](https://docs.aws.amazon.com/ja_jp/codedeploy/latest/userguide/instances.html)
* [デプロイ設定の使用](https://docs.aws.amazon.com/ja_jp/codedeploy/latest/userguide/deployment-configurations.html)
* [アプリケーションの使用](https://docs.aws.amazon.com/ja_jp/codedeploy/latest/userguide/applications.html)
* [デプロイグループの使用](https://docs.aws.amazon.com/ja_jp/codedeploy/latest/userguide/deployment-groups.html)
* [アプリケーションリビジョンの操作](https://docs.aws.amazon.com/ja_jp/codedeploy/latest/userguide/application-revisions.html)

※ 新しい今ソーツデザインの概念では、デプロイの作成 = デプロイの実行

### AppSpec file
* AppSpec file は、ファイルで定義されている一連のライフサイクルイベントフックとして、各デプロイを管理するために使用される


## IAM (AWS Identity and Access Management)
WS リソースへのアクセスを安全にコンソールするためのウェブサービスです。

IAM を使用して、リソースを使用するために認証 (サインイン) され、許可された (アクセス許可を持つ) ユーザーを制御します。

### IAMの機能
- AWS アカウントへの共有アクセス
- 詳細なアクセス権限
- Amazon EC2 で動作するアプリケーションから AWS リソースへの安全なアクセス
- 多要素認証 (MFA)
- ID フェデレーション
- 保証のための ID 情報
- PCI DSS への準拠
- 多くの AWS サービスとの統合
- 結果整合性
- 使用料無料


### ID
IAM ユーザー
 * アカウントID, アカウント名, パスワードでログイン
IAM グループ
 * IAM ユーザーの集合
 * グループを使用してユーザーの集合に対してアクセス許可を指定、ユーザーのアクセス許可を管理
IAM ロール
  * AWSでできることとできないことを決定するアクセス許可ポリシーが適用されるID
  * IAMユーザと同様、AWSで許可/禁止する操作を決めるアクセス権限ポリシーが関連付けられているAWSアイデンティティ
  * 信頼できるエンティティにアクセス権限を付与する
    * 別のアカウントの IAM ユーザー
    * AWS のリソースでアクションを実行する必要がある、EC2 インスタンスで実行されるアプリケーションコード
    * 機能を提供するためにお客様のアカウントのリソースを操作する必要がある AWS のサービス
    * SAML を使用した ID フェデレーションを使用する企業内ディレクトリからのユーザー

## 開始方法

### 設定
[開始方法](https://docs.aws.amazon.com/ja_jp/IAM/latest/UserGuide/getting-started.html)
* [最初の IAM 管理者のユーザーおよびグループの作成](https://docs.aws.amazon.com/ja_jp/IAM/latest/UserGuide/getting-started_create-admin-group.html)
* [IAM が委任した最初のユーザーおよびグループの作成](https://docs.aws.amazon.com/ja_jp/IAM/latest/UserGuide/getting-started_create-delegated-user.html)
* [ユーザーがアカウントにサインインする方法](https://docs.aws.amazon.com/ja_jp/IAM/latest/UserGuide/getting-started_how-users-sign-in.html)
