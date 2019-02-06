# プロジェクト作成

適当なプロジェクトフォルダを作成して初期化する。

```
> mkdir sample
> cd sample
> gitbook init
```

#### プラグイン

npm パッケージをインストールする。

```
> npm install gitbook-plugin-livereload
```

プロジェクトのルートに `book.json` を作成する。

```json
{
  "plugins": [
    "-sharing",
    "hide-published-with",
    "livereload"
  ]
}
```

プラグインをインストールする。

```
> gitbook install
```
