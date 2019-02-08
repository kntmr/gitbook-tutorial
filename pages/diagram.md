# UML

ここでは、PlantUML で UML を記述する。事前に Graphviz をインストールして、環境変数 `GRAPHVIZ_DOT` (dot.exe ファイルのパス) を設定する。

[Graphviz - Graph Visualization Software](https://graphviz.gitlab.io/_pages/Download/Download_windows.html)

#### プラグイン

`book.json` にプラグインと設定を追加する。

```json
{
  "plugins": [
    "-sharing",
    "hide-published-with",
    "livereload",
    "uml"
  ],
  "pluginsConfig": {
    "uml": {
      "charset" : "UTF-8"
    }
  }
}
```

プラグインをインストールする。

```
> gitbook install
```

#### PlantUML

PlantUML の記法については、[PlantUML 概要](http://plantuml.com/ja/) を参照。

#### プラグインインストールでエラーになる場合

> Error: node-plantuml@0.6.2 postinstall: node scripts/get-plantuml-jar.js

個別にパッケージをインストールして回避する。

```
> cd node_modules
> git clone https://github.com/vowstar/gitbook-plugin-uml.git
```

gitbook-plugin-uml の `package.json` を変更する。

```json
"dependencies": {
  // ... (略)
  "node-plantuml": "^0.6.2" // ^0.6.2 ⇒ ^0.7.0 に書き換える
}
```

```
> cd gitbook-plugin-uml
> npm install
```

プロジェクトのルートに戻って、`gitbook install` を実行する。
