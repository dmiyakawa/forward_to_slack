# これは何

メールをなんとなくSlackのチャンネルへ転送する。
SlackのIncoming Webhooksを使う。

    e.g. (/etc/aliases へ以下のように追加する)

    slack:  "|/path/to/forward_to_slack https://hooks.slack.com/services/..."

いくらかオプションがある。詳細は-hかコード参照

 * -h ... help
 * -s ... syslog
 * -r ... stream (stderr)
 * -d ... debug

特別作り込むつもりはない。

# 動作環境とか

 * Python 3系が前提。
   * Python 3.5以降 + Postfx + /etc/aliases で動作確認
 * 外部ライブラリ
   * requests


# License

MIT


# 参考

愚直にIncoming Webhooksを使っているだけ。
https://api.slack.com/incoming-webhooks

有料プランであればEmail appを使えば良い
https://get.slack.help/hc/en-us/articles/206819278-Send-emails-to-Slack

このレベルだとどちらかと言うと賢くMIMEをパースするほうが面倒な気が……。

参考: https://github.com/dmiyakawa/python_capture_mail
