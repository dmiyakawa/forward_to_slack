# これは何

メールをなんとなくSlackのチャンネルへ転送する。

    e.g. (/etc/aliases へ以下のように追加する)

    slack:  "|/path/to/forward_to_slack https://hooks.slack.com/services/..."

いくらかオプションがある。詳細は-hかコード参照

 * -h ... help
 * -s ... syslog
 * -r ... stream (stderr)
 * -d ... debug

# 動作環境とか

 * Python 3系が前提。
   * Python 3.5以降 + Postfx + /etc/aliases で動作確認
 * 外部ライブラリ
   * requests


# License

MIT
