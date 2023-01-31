# Flutter サンプルアプリ
Bitrise onboarding 用のFlutterプロジェクト
- Flutter サンプルアプリ
- bitrise.ymlファイル

## カリキュラム
1.  ダッシュボードの紹介
    - [最初のアプリ追加](https://devcenter.bitrise.io/en/getting-started/adding-your-first-app.html)
    - [flutterアプリのオンボーディング設定](https://devcenter.bitrise.io/en/getting-started/getting-started-with-flutter-apps.html)
    - [BitriseアカウントにGithub、appleと連携](https://devcenter.bitrise.io/en/accounts/connecting-to-services/connecting-your-github-gitlab-bitbucket-account-to-bitrise.html#connecting-your-github-gitlab-bitbucket-account-to-bitrise)
    
2. Workflowエディター紹介
    - [Code signing設定](https://devcenter.bitrise.io/en/code-signing.html)
        - [Android Code signing](https://devcenter.bitrise.io/en/code-signing/android-code-signing.html)
        - [iOS Code signing](https://devcenter.bitrise.io/en/code-signing/ios-code-signing.html)
    - [EnvVar設定（環境関数設定）](https://devcenter.bitrise.io/en/builds/environment-variables.html
)
    - [シークレット設定（証明書など）](https://devcenter.bitrise.io/en/builds/secrets.html)
    - [primary workflowの設定](https://devcenter.bitrise.io/en/steps-and-workflows.html)
    - [ビルドマシーン紹介](https://devcenter.bitrise.io/en/infrastructure/build-machines/build-machine-types.html)
    - [スタック設定](https://devcenter.bitrise.io/en/builds/configuring-build-settings/setting-the-stack-for-your-builds.html#setting-the-stack-in-the-workflow-editor)
    - [workflow iOS サンプルレシピ](https://devcenter.bitrise.io/en/steps-and-workflows/workflow-recipes-for-ios-apps.html)
    - [workflow flutter サンプルレシピ](https://devcenter.bitrise.io/en/steps-and-workflows/workflow-recipes-for-cross-platform-apps.html)
    - [ローカルデバッグコマンドツール紹介-Bitrise CLI](https://devcenter.bitrise.io/en/builds/build-data-and-troubleshooting/debugging-your-build-on-your-own-machine.html)
3. テスト
    - [flutter Unitテスト](https://devcenter.bitrise.io/en/getting-started/getting-started-with-flutter-apps.html#testing-a-flutter-app)
    - デバイステスト
        - [iOSデバイステスト](https://devcenter.bitrise.io/en/testing/device-testing-for-ios.html)
        - [Androidデバイステスト](https://devcenter.bitrise.io/en/testing/device-testing-for-android.html)
    - [oAuth1認証必要の場合のテスト](https://softwareengineering.stackexchange.com/questions/413182/store-oauth-2-0-tokens-for-use-in-testing-and-ci-cd)
    - 2FA認証必要の場合 (2FA auth is not really suited for CI systems as there is no user interaction)
    - 位置情報関連のテスト[参考１](https://github.com/udevsharold/locsim), [参考２](https://itnext.io/simulate-debugging-location-in-ios-24496cbbc9d9)
    - [現在時刻に依存するテスト](https://www.bitrise.io/integrations/steps/set-macos-timezone)
    - API関連のテスト [(Mock API使用を推薦)](https://stackoverflow.com/questions/55409978/how-to-mock-http-request-in-flutter-integration-test)
    - [音声関連のテスト](https://discuss.bitrise.io/t/how-to-create-a-virtual-audio-output-device-on-mac-os-stacks/1119)
4. ビルド
    - [Build Pipeline(Beta)の紹介](https://devcenter.bitrise.io/en/builds.html)
    - [flutterビルド](https://devcenter.bitrise.io/en/getting-started/getting-started-with-flutter-apps.html#deploying-a-flutter-app)
    - [Build Artifact]
5. デプロイ
    - [デプロイ設定](https://devcenter.bitrise.io/en/deploying.html)
    - [firebaseへのデプロイ-iOS](https://devcenter.bitrise.io/en/steps-and-workflows/workflow-recipes-for-ios-apps/-ios--deploy-to-firebase-app-distribution.html)
    - [firebaseへのデプロイ-Android](https://devcenter.bitrise.io/en/steps-and-workflows/workflow-recipes-for-ios-apps/-ios--deploy-to-firebase-app-distribution.html)
    - [Testflightへのデプロイ](https://devcenter.bitrise.io/en/steps-and-workflows/workflow-recipes-for-android-apps/-android--deploy-to-firebase-app-distribution.html)
    - [Play storeへのデプロイ](https://devcenter.bitrise.io/en/deploying/android-deployment/deploying-android-apps-to-bitrise-and-google-play.html)
    - [App Store Connectへのデプロイ](https://devcenter.bitrise.io/en/deploying/ios-deployment/deploying-an-ios-app-to-app-store-connect.html)
    - [Release Management(Beta)の紹介](https://devcenter.bitrise.io/en/deploying/release-management.html)

6. セキュリティ関連やサードパーティサービス統合などのトピック
    - [VPN設定](https://devcenter.bitrise.io/en/builds/connecting-to-a-vpn-during-a-build.html#using-cisco-vpn)
    - [ネットアクセス制限設定](https://devcenter.bitrise.io/en/infrastructure/build-machines/configuring-your-network-to-access-our-build-machines.html)
    - [Slack統合](https://devcenter.bitrise.io/en/builds/configuring-build-settings/configuring-slack-integration.html)



