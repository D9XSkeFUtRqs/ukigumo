# Ukigumo

[Mastodon](https://github.com/tootsuite/mastodon)のデスクトップクライアント「[Mstdn.app](https://github.com/rhysd/Mstdn)」を某所風にするスタイルシート

## 導入

[本家のRead Me](https://github.com/rhysd/Mstdn#readme)が英語 + 間違っている（？）箇所があるため簡単に解説。
macOSとLinuxは分からない世界なので間違ってたらごめんなさい。

### Mstdn.appのインストール

#. [ここの「Downloads」](https://github.com/rhysd/Mstdn/releases)から各OS用のファイルをダウンロード（Windowsだったら多分「Mstdn-win32-x64-x.x.x.zip」）
#. 適当なところに展開
#. Mstdn.exeを起動すると「Please write configulation in JSON」と出て、config.jsonが開く
#. config.jsonを以下のように書き換えて、保存する
    + "chromium_sandbox": "true"　→　"false"
    + "name": ""　→　"（自分のアカウント名）"
    + "host": ""　→　"（自分のインスタンス名）"
    + "default_page": "/web/timelines/home"　→　"/web/getting-started"
#. Mstdn.exeをもう一度起動すると、アプリが開く

### スタイルシートの適用

#. ダウンロード
#. config.jsonが存在する場所に、user.cssを移動する
#. Mstdn.exeを起動する
