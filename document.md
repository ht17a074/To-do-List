# To-do List

この To-do List は HTML と CSS, JavaScript の 3 つで構成される Web アプリケーションです。このアプリケーションの画面上で必要な機能は、

- To-do の追加
- To-do の削除
- 選択された To-do の削除

になります。

このアプリケーションの To-do データは、
Web Storage API の localStorage を使用してローカル環境(ブラウザ)に保存します。
この localStorage はオリジン単位でデータを保存するため、
開発時に Web サーバーの起動が必要になります。

(オリジンとは、URL の「スキーム://ホスト:ポート」の組み合わせのことです。)

## 貢献方法

- このプロジェクトをフォークする
- 学籍番号のブランチを作成して切り替える
- `submit/` 内に学生番号(小文字)のディレクトリを作成
  - 例: `ht99a999`
- 上記で作成したディレクトリ内に、`template/` の中身をコピー
  - 例
  - ht99a999/
    - index.html
    - main.js
    - ress.css
    - style.css
- [サーバーを起動](#%e3%82%b5%e3%83%bc%e3%83%90%e3%83%bc%e3%81%ae%e8%b5%b7%e5%8b%95%e6%96%b9%e6%b3%95)
- 「[template からコピーしてきたファイルに加える変更](#template-%e3%81%8b%e3%82%89%e3%82%b3%e3%83%94%e3%83%bc%e3%81%97%e3%81%a6%e3%81%8d%e3%81%9f%e3%83%95%e3%82%a1%e3%82%a4%e3%83%ab%e3%81%ab%e5%8a%a0%e3%81%88%e3%82%8b%e5%a4%89%e6%9b%b4)」を見て作業
- 変更をコミットする
- ブランチをプッシュ
- プルリクエストを作成

## サーバーの起動方法

開発時には Web サーバーの起動が必要ですが、どんな方法で起動しても構いません。
ここでは、[Visual Studio Code](https://azure.microsoft.com/ja-jp/products/visual-studio-code/) を用いたサーバーの起動方法を紹介します。

- Visual Studio Code に `Live Server` という拡張機能を導入
  - Visual Studio Code の左側から拡張機能のタブを開いて検索
  - Ctrl + Shift + X でも拡張機能のタブを表示できる
- html ファイルが入っているディレクトリを Visual Studio Code で開く
  - ドラッグ & ドロップで開けます
- 右下の `Go Live` をクリックしてサーバーを起動
  - 起動時にポート番号が競合してなければ <http://localhost:5500/> でアクセス可能
  - 停止するには右下の `Port : xxxx` と書いてるところを選択

## template からコピーしてきたファイルに加える変更

### HTML: inedx.html

- 22 行目: [Delete selected items] ボタン
  - 選択された項目を削除する関数 `deleteSelected()` を呼び出すように

### CSS: style.css(ress.css は触らない)

- 大見出し (h1) を中央揃えに
- body に対して Google Fonts を導入

### JavaScript: main.js

- 特になし (必要な関数は実装済み)
