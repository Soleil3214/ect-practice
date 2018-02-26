# ect_template
テンプレートエンジン「ECT」を使用したテンプレート


## バージョン

### ver. 1.0.0
基本的なテンプレートセット


### 使い方と仕様


#### ＜使い方＞
  1. nodeをインストール
  2. 作業ディレクトリに移動し、コマンド「npm install」で必要なパッケージをインストール
  3. コマンド「gulp」でローカルサーバー起動

#### ＜仕様＞
  * /src/templates/pages/以下の.ectファイル、/src/styles/以下の.scssファイル、/src/js/以下のjsファイルを上書き保存すると、自動ビルドとブラウザリロードが始まります。  
  ＊/src/templates/の/pages/以外を編集した場合には、ターミナル上で「Ctr+C」で一旦gulpを止めてから、再びターミナル上で「gulp」コマンドを叩いて下さい。  
  ＊処理が重い場合やPCのスペック・メモリの都合でリロードしても変更が反映しきれない場合があります。  
  その場合には手動でブラウザをリロードして下さい。
  * /src/以下のファイルを編集すると、/src/と同じ階層に「/dist/」フォルダが自動的に生成されます。  
  * ectのエラーが出ると、/dist/内に「.ect」のファイルが出力されます。  
  エラーを取り除き、dist内のectファイルを削除した後、「gulp」コマンドを使用してビルドを行って下さい。
  ＊画像フォルダは/dist内に作成して下さい。  
  例：/dist/images/  
  ＊サーバーにアップロードするのは/dist/内のファイルのみ。