# nodejs-hello-world

Node.jsを用いたHello Worldプログラム。

## 推奨開発環境

- Node.js v12.14.0 以降
- Visual Studio Code 1.45.1 以降

## プロジェクト構成

- `.`
  - `.vscode` <- Visual Studio向けプロジェクト設定群
    - `extensions.json` <- 開発時に推奨される拡張機能一覧
    - `launch.json` <- 起動設定の記述されたファイル
  - `.editorconfig` <- コードの記述スタイル設定。推奨拡張機能をインストールすると適用される
  - `.gitignore` <- Gitコミット時に無視するファイル一覧
  - `index.js` <- プログラム本体
  - `package-lock.json` <- npm install実行後のバージョン指定ファイル
  - `package.json` <- プロジェクトの設定と依存関係
  - `README.md` <- 本ファイル。使い方や開発に役立つ情報を記述する。

## 実行方法

### Visual Studio Codeを利用する場合

`.vscode/launch.json` に設定が記述されているため、エディタから直接実行できます。  
左側のアクティビティバー内にある `Run` を展開し、Configurationとして `Launch Program` を選択し、実行ボタンを押下してください。

> [![Image from Gyazo](https://t.gyazo.com/teams/kiganix/b29aa4df375209a01dd4590f831662dd.png)](https://kiganix.gyazo.com/b29aa4df375209a01dd4590f831662dd)

エディタの統合ターミナル内に、下記のような表示がされるはずです。

```
/opt/nodejs/lts/bin/node --inspect-brk=***** index.js 
︙
Hello World!
︙
```
