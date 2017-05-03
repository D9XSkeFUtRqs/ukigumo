# Ukigumo

[Mastodon](https://github.com/tootsuite/mastodon)のデスクトップクライアント「[Mstdn](https://github.com/rhysd/Mstdn)」を某所風にするスタイルシート

バグ、デザイン案、質問などは[Issueページ](https://github.com/D9XSkeFUtRqs/ukigumo/issues)または[こちら](https://ftb.moe/@D9XSkeFUtRqs)から気軽にどうぞ

## 導入

[MstdnのREADME](https://github.com/rhysd/Mstdn#readme)が英語 + 間違っている（？）箇所があるため簡単に解説。

macOSとLinuxは分からない世界なので間違ってたらごめんなさい。

### Mstdn.appのインストール

1. [MstdnのReleaseページ](https://github.com/rhysd/Mstdn/releases)から各OS用のファイルをダウンロード、適当なところに展開<br>（Windowsだったら多分「Mstdn-win32-x64-x.x.x.zip」）
    + 私の環境（Windows10）では何故かv0.2.4が起動しない…<br>もし同様であればv0.2.3を試してみてください
1. Mstdn.exeを起動すると「Please write configulation in JSON」と出て、config.jsonが開く
1. config.jsonを以下のように書き換えて、保存する
    + `"chromium_sandbox": "true"`　→　`"false"`
    + `"name": ""`　→　`"（自分のアカウント名）"`
    + `"host": ""`　→　`"（自分のインスタンス名）"`
1. Mstdn.exeをもう一度起動すると、アプリが開く

### スタイルシートの適用

1. [Releaseページ](https://github.com/D9XSkeFUtRqs/ukigumo/releases)からダウンロードし、展開
1. インストール時に書き換えたconfig.jsonが存在するフォルダを探す<br>config.jsonがあるのは多分以下のあたり
    + Windows：`%APPDATA%\Mstdn`
    + macOS：`~/Library/Application\ Support/Mstdn`
    + Linux：`~/.config/Mstdn`
1. そのフォルダにダウンロードしたuser.cssを移動する
1. config.jsonを以下のように書き換えて、保存する
    + `"default_page": "/web/timelines/home"`　→　`"/web/getting-started"`
1. Mstdn.exeを起動する
