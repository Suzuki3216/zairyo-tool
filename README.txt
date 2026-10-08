材料取りツール  ホーム画面アプリ（PWA）セット  Ver.1-30

■ 入っているファイル（すべて同じフォルダに置いてください）
  index.html            ツール本体
  manifest.webmanifest  アプリの名前・アイコンなどの設定
  sw.js                 オフライン起動のための設定
  icon-192.png / icon-512.png / apple-touch-icon.png   アプリのアイコン

■ 使い方の流れ
  1. このフォルダ一式を、https:// で公開できる場所に置く（下記 A または B）
  2. スマホのブラウザでそのアドレスを開く
  3. 「ホーム画面に追加」する（下記）

■ A. GitHub Pages（無料）に置く
  1. https://github.com でアカウントを作成してログインする
  2. 右上の「＋」→「New repository」。名前を例えば zairyo-tool とし、Public を選んで作成する
  3. 「uploading an existing file」を押し、このフォルダの中のファイルを全部ドラッグして「Commit changes」
  4. 「Settings」→「Pages」→ Branch を「main」、フォルダを「/(root)」にして「Save」
  5. 数分後、画面に表示される https://（ユーザー名）.github.io/zairyo-tool/ が、アプリのアドレス
  ※ Public にすると、アドレスを知っている人は誰でも開けます（入力した内容はスマホの中にだけ残り、外部には送られません）

■ B. Netlify Drop（無料・いちばん簡単）に置く
  1. https://app.netlify.com/drop を開く（アカウント登録が必要な場合があります）
  2. このフォルダごと、画面の枠にドラッグ＆ドロップする
  3. 表示された https://～.netlify.app が、アプリのアドレス

■ ホーム画面に追加する
  iPhone（Safari で開く）  共有ボタン（□に↑）→「ホーム画面に追加」→「追加」
  Android（Chrome で開く） 右上の「⋮」→「アプリをインストール」または「ホーム画面に追加」

■ ツールを更新するとき
  1. 新しい index.html に差し替える
  2. sw.js の VERSION の数字（例 zairyo-v1-30）を変える
  3. 公開し直す。スマホは次の起動のあと、新しい版に切り替わります

■ 注意
  ・データ保存：iPhone／Android では、共有メニューが開きます。「ファイルに保存」などを選んでください
  ・入力内容はアプリを閉じると消えます。続きは「データ保存」→「データ読込」で
  ・初回はインターネット接続が必要です。2回目以降は、通信がなくても起動できます
