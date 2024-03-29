# Bitrise オンボーディングトレーニング
このリポジトリには、Bitriseのオンボーディングトレーニング用の資料が含まれています。

- Flutter サンプルアプリ

- `bitrise.yml`：bitrise.ymlファイルサンプル

- `Chap*.md`：各章のトレーニング資料

- 2/09 Chap1 60 mins
- 2/13 Chap2 59 mins
- 2/20 Chap3 35 mins
- 3/06 Chap4 62 mins
- 3/09 Chap5 62 mins
- 3/13 Chap6 40 mins
- 3/16 Q&A 33 mins


# カリキュラム
## 1. [Bitriseの基本紹介](Chap1.md)
- ダッシュボードの紹介
- [BitriseアカウントにGitアカウントと連携](https://devcenter.bitrise.io/en/accounts/connecting-to-services/connecting-your-github-gitlab-bitbucket-account-to-bitrise.html#connecting-your-github-gitlab-bitbucket-account-to-bitrise)

- [apple developerアカウントと連携](https://devcenter.bitrise.io/en/accounts/connecting-to-services/apple-services-connection.html)

- [最初のアプリ追加](https://devcenter.bitrise.io/en/getting-started/adding-your-first-app.html)

- [Flutterアプリのオンボーディング設定](https://devcenter.bitrise.io/en/getting-started/getting-started-with-flutter-apps.html)

## 2. [Workflowエディター紹介](Chap2.md)

- [ステップの紹介](https://devcenter.bitrise.io/en/steps-and-workflows/introduction-to-steps.html)

    - アドバンス設定
    - https://devcenter.bitrise.io/en/steps-and-workflows/introduction-to-steps/skipping-steps.html
    - https://devcenter.bitrise.io/en/steps-and-workflows/introduction-to-steps/enabling-or-disabling-a-step-conditionally.html
    - https://devcenter.bitrise.io/en/steps-and-workflows/introduction-to-steps/setting-a-time-limit-for-steps.html
    - Hanging Build abortion https://devcenter.bitrise.io/en/steps-and-workflows/introduction-to-steps/detecting-and-aborting-hanging-steps.html
    - Custom Step reference: https://devcenter.bitrise.io/en/references/steps-reference/step-reference-id-format.html

- [workflowの紹介](https://devcenter.bitrise.io/en/steps-and-workflows/introduction-to-workflows.html)

    - アドバンス設定
    - Chaining Workflows: https://devcenter.bitrise.io/en/steps-and-workflows/introduction-to-workflows/managing-workflows.html
    - [別のアプリからワークフローをコピー](https://devcenter.bitrise.io/en/steps-and-workflows/introduction-to-workflows/copying-workflows-from-one-app-to-another.html
)

- [Code signing設定](https://devcenter.bitrise.io/en/code-signing.html)
    - [Android Code signing](https://devcenter.bitrise.io/en/code-signing/android-code-signing.html)
    - [iOS Code signing](https://devcenter.bitrise.io/en/code-signing/ios-code-signing.html)
- [EnvVar設定（環境関数設定）](https://devcenter.bitrise.io/en/builds/environment-variables.html)
- [シークレット設定（パスワードなど）](https://devcenter.bitrise.io/en/builds/secrets.html)
- [primary workflowの設定](https://devcenter.bitrise.io/en/steps-and-workflows.html)
- [ビルドマシーン紹介](https://devcenter.bitrise.io/en/infrastructure/build-machines/build-machine-types.html)
- [スタック設定](https://devcenter.bitrise.io/en/builds/configuring-build-settings/setting-the-stack-for-your-builds.html#setting-the-stack-in-the-workflow-editor)
- [workflow iOS サンプルレシピ](https://devcenter.bitrise.io/en/steps-and-workflows/workflow-recipes-for-ios-apps.html)
- [workflow flutter サンプルレシピ](https://devcenter.bitrise.io/en/steps-and-workflows/workflow-recipes-for-cross-platform-apps.html)
- [キャッシュの最適化](https://devcenter.bitrise.io/en/steps-and-workflows/generic-workflow-recipes/make-caching-efficient-for-pull-request-builds.html)

## 3. デバッグとテスト
- [start/schedule buildとRebuildボタンの紹介](https://devcenter.bitrise.io/en/builds/environment-variables.html#setting-a-custom-env-var-when-starting-a-build)
- [リモートアクセス](https://devcenter.bitrise.io/en/builds/build-data-and-troubleshooting/remote-access.html)
- [ローカルデバッグコマンドツール紹介-Bitrise CLI](https://devcenter.bitrise.io/en/builds/build-data-and-troubleshooting/debugging-your-build-on-your-own-machine.html)
- [flutter Unitテスト](https://devcenter.bitrise.io/en/getting-started/getting-started-with-flutter-apps.html#testing-a-flutter-app)
- デバイステスト
    - [iOSデバイステスト](https://devcenter.bitrise.io/en/testing/device-testing-for-ios.html)
    - [Androidデバイステスト](https://devcenter.bitrise.io/en/testing/device-testing-for-android.html)
- [oAuth1認証必要の場合のテスト](https://softwareengineering.stackexchange.com/questions/413182/store-oauth-2-0-tokens-for-use-in-testing-and-ci-cd)
- 2FA認証必要の場合 (2FA auth is not really suited for CI systems as there is no user interaction)
- 位置情報関連のテスト[参考１](https://github.com/udevsharold/locsim), [参考２](https://itnext.io/simulate-debugging-location-in-ios-24496cbbc9d9)
- API関連のテスト [(Mock API使用を推薦)](https://stackoverflow.com/questions/55409978/how-to-mock-http-request-in-flutter-integration-test)
- [現在時刻に依存するテスト](https://www.bitrise.io/integrations/steps/set-macos-timezone)
- [音声関連のテスト](https://discuss.bitrise.io/t/how-to-create-a-virtual-audio-output-device-on-mac-os-stacks/1119)

## 4. ビルド
- [Selective build](https://devcenter.bitrise.io/en/builds/configuring-build-settings/selective-builds.html)
- [Rolling Build](https://devcenter.bitrise.io/en/builds/configuring-build-settings/rolling-builds.html)
- [Bitrise Start Buildステップ](https://devcenter.bitrise.io/en/steps-and-workflows/generic-workflow-recipes/start--parallel--builds-from-the-workflow.html)
- With Git provider
    - [Report build status back to Git provider](https://devcenter.bitrise.io/en/builds/configuring-build-settings/reporting-the-build-status-to-your-git-hosting-provider.html)
    - [Github check](https://devcenter.bitrise.io/en/builds/build-data-and-troubleshooting/bitrise-checks-on-github.html#enabling-github-checks-on-bitrise)
- [Build Pipeline(Beta)の紹介](https://devcenter.bitrise.io/en/builds.html)
- [Pipeline editor](https://damienbitrise.github.io/Pipeline-UI/)
- [flutterビルド](https://devcenter.bitrise.io/en/getting-started/getting-started-with-flutter-apps.html#deploying-a-flutter-app)

## 5. デプロイ
- [デプロイ設定](https://devcenter.bitrise.io/en/deploying.html)
- [Play storeへのデプロイ](https://devcenter.bitrise.io/en/deploying/android-deployment/deploying-android-apps-to-bitrise-and-google-play.html)
- [Firebaseへのデプロイ-Android](https://devcenter.bitrise.io/en/steps-and-workflows/workflow-recipes-for-android-apps/-android--deploy-to-firebase-app-distribution.html)
- [App Store Connect/Testflightへのデプロイ](https://devcenter.bitrise.io/en/deploying/ios-deployment/deploying-an-ios-app-to-app-store-connect.html)
- [Firebaseへのデプロイ-iOS](https://devcenter.bitrise.io/en/steps-and-workflows/workflow-recipes-for-ios-apps/-ios--deploy-to-firebase-app-distribution.html)
- [Release Management(Beta)の紹介](https://devcenter.bitrise.io/en/deploying/release-management.html)
- [Shipの紹介](https://devcenter.bitrise.io/en/deploying/deploying-with-ship.html)

# 6. Insights、セキュリティ関連やサードパーティサービス統合などのトピック
- [Insights](https://devcenter.bitrise.io/en/insights.html)
- [API](https://devcenter.bitrise.io/en/api.html)
- [VPN設定](https://devcenter.bitrise.io/en/builds/connecting-to-a-vpn-during-a-build.html#using-cisco-vpn)
- [ネットアクセス制限設定](https://devcenter.bitrise.io/en/infrastructure/build-machines/configuring-your-network-to-access-our-build-machines.html)
- Slack統合:
    - https://devcenter.bitrise.io/en/builds/configuring-build-settings/configuring-slack-integration.html
    - https://devcenter.bitrise.io/en/steps-and-workflows/generic-workflow-recipes/-ios-android--send-build-status-to-slack.html
    - QR code: https://devcenter.bitrise.io/en/steps-and-workflows/generic-workflow-recipes/-ios-android--send-qr-code-to-slack.html




