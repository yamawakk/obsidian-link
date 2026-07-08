# obsidian-link — Slack通知からObsidianを開くための中継ページ

これは何：Slackのメッセージは `obsidian://…`（Obsidianアプリを直接開く合図）をリンクにしてくれない。
そこで、この1枚のページ（https のリンク＝Slackで押せる）を経由して Obsidian に転送する。

- 使い方：`https://yamawakk.github.io/obsidian-link/#v=保管庫名&f=ファイルパス`
- ファイル名は `#` より後ろに載せる＝**ブラウザの中だけで処理され、サーバーには送られない**。
- このリポジトリに個人情報・データは一切置かない（この転送ページ1枚だけ）。
- 本体の仕組み：life-hub（非公開リポジトリ）の `setup/hooks/notify-doc-update.py` がリンクを組み立てる。
