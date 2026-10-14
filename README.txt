千式コード Webアプリ版（ホーム画面に追加して遊べる形）

■ 入っているもの
  index.html            ゲーム本体
  manifest.webmanifest  アプリの名前・アイコンの情報
  sw.js                 オフラインでも開けるようにするしくみ
  icon-*.png / favicon-32.png  アイコン

■ GitHub Pages で公開する手順
  1. GitHub で新しいリポジトリを作る（例：senshiki-code、Public）
  2. 「Add file」→「Upload files」で、このフォルダの中身をすべてアップロードして Commit
  3. リポジトリの Settings → Pages → Branch を「main」「/(root)」にして Save
  4. 数分後に表示される https://（ユーザー名）.github.io/senshiki-code/ を開く

■ スマートフォンにインストールする
  iPhone（Safari）：共有ボタン →「ホーム画面に追加」
  Android（Chrome）：メニュー（︙）→「アプリをインストール」または「ホーム画面に追加」

■ セーブデータについて
  アプリ版とブラウザ版ではセーブデータが別々です。
  もとのほうの「設定」→「データの引っ越し」→「データをコピー」、
  移す先の同じ場所に貼りつけて「読み込む」で移せます。

■ 更新するとき
  新しい index.html を同じ場所に上書きアップロードしてください。
  アプリは次に開いたときに新しい版を読み込みます（つながっていないときは前の版で動きます）。

■ 通信対戦について
  2台の端末を同じWi-Fiにつなぎ、メニューの「通信対戦」から遊びます。
  QRコードをカメラで読み取るには、GitHub Pages など https のページで開いてください
  （ファイルを直接開いたときは、合図をコピーして貼りつけてつなげます）。
  使っているライブラリ：qrcode-generator（MIT License）、jsQR（Apache License 2.0）。
