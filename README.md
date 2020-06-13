# nodejs-hello-world

Node.jsを用いたHello Worldプログラム。

## 推奨開発環境

- Node.js v12.14.0 以降
- Visual Studio Code 1.45.1 以降

## プロジェクトのclone

### Visual Studio Codeを利用する場合

Visual Studio Codeのメニューから `Terminal` -> `New Terminal` と進み、統合ターミナルを開いてください。

[![Image from Gyazo](https://t.gyazo.com/teams/kiganix/515d289467723bff9e9cecd161ddde74.png)](https://kiganix.gyazo.com/515d289467723bff9e9cecd161ddde74)

ターミナルを開いたら、下記のようにコマンドを実行し、プロジェクトをcloneします。

```shell
git clone https://github.com/seisahachioji/nodejs-hello-world.git
```

cloneが完了したら、メニューから `File` -> `Open` と進み、cloneしたディレクトリを選択し `OK` を押下してください。

> [![Image from Gyazo](https://t.gyazo.com/teams/kiganix/7da70bd72627375b304b4b0301121752.png)](https://kiganix.gyazo.com/7da70bd72627375b304b4b0301121752)

> [![Image from Gyazo](https://t.gyazo.com/teams/kiganix/f7f6933b4331ee8d02afa1ef4c21b6d2.png)](https://kiganix.gyazo.com/f7f6933b4331ee8d02afa1ef4c21b6d2)
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

#### プロジェクトの初期化

Node.jsを用いたNPMプロジェクトであるため、プロジェクトの初期化を行ってください。  
なお、本プロジェクトは今のところ外部の依存関係を持たないため、実行しても特段変化は起きません。

統合ターミナルを開き、下記のように実行します。

```shell
npm install
```

#### プログラム本体の実行

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
