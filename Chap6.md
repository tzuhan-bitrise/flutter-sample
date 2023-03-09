# Insights、セキュリティ関連やサードパーティサービス統合などのトピック

# [VPN設定](https://devcenter.bitrise.io/en/builds/connecting-to-a-vpn-during-a-build.html#using-cisco-vpn)
[VPNC](https://linux.die.net/man/8/vpnc)というCisco 3000 VPN Concetratorが提供しているVPNクライアントツールを使います。


- ワークフローに `Cisco VPN connect` ステップを追加
- vpnc.conf ファイルにVPNクライアントを設定
- `Command line option` にvpncへのコマンドオプションを入力


また、ファイアウォールのホワイトリストにBitriseマシンのIPアドレスを追加していただく必要もあります。
[BitriseマシンのIPアドレスリスト](https://devcenter.bitrise.io/en/infrastructure/build-machines/configuring-your-network-to-access-our-build-machines.html#ip-addresses-for-the-bitrise-build-machines)


# [Insights](https://devcenter.bitrise.io/en/insights.html)

# [API](https://devcenter.bitrise.io/en/api.html)


# [ネットアクセス制限設定](https://devcenter.bitrise.io/en/infrastructure/build-machines/configuring-your-network-to-access-our-build-machines.html)

# Slack統合
- https://devcenter.bitrise.io/en/builds/configuring-build-settings/configuring-slack-integration.html
- https://devcenter.bitrise.io/en/steps-and-workflows/generic-workflow-recipes/-ios-android--send-build-status-to-slack.html
- QR code: https://devcenter.bitrise.io/en/steps-and-workflows/generic-workflow-recipes/-ios-android--send-qr-code-to-slack.html
