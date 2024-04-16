##NODE.jsを使う目的
### 新しい仕様のJavaScriptまたはTypeScriptでクライアントサイドのプログラムを書きたい
年々新しくなるjavascriptの仕様に既存のブラウザが追いついてこれないと問題が起こる
そのためBabelなどのトランスパイラが　「新しい仕様で書いたJavaScriptファイル」を機械的に「旧仕様（ES5）のJavaScriptファイル」に変換（トランスパイル）する
それを動かすための環境としてNode.jsが使われる

###Webアプリケーションが作りたい
Javascriptの実行環境として使われる
Node.js（実行環境）＋Javascript（言語）＋Express,Next.js（Webフレームワーク）
Node.jsがWebサーバーの代わりに直接HTTPリクエストを受け取り、処理をする
（実際にはNode.jsのみだとWebサーバとしては少し機能が物足りないので、その前段にApacheやnginxをリバースプロキシとして置く構成が多い）
