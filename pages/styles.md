# スタイル

ここでは、HTML と PDF のスタイル変更や便利なプラグインについて記載する。今回利用する `expandable-chapters` は子メニューを開閉するためのプラグイン。

#### プラグイン

`book.json` にプラグインと設定を追加する。

```json
{
  "plugins": [
    "-sharing",
    "hide-published-with",
    "livereload",
    "uml",
    "expandable-chapters"
  ],
  "pluginsConfig": {
    "uml": {
      "charset" : "UTF-8"
    }
  },
  "styles": {
    "website": "styles/website.css",
    "pdf": "styles/pdf.css"
  }
}
```

プラグインをインストールする。

```
> gitbook install
```

#### スタイル変更

`book.json` の `styles` に指定した css ファイルでスタイルを上書きする。今回は主にメニューや h2, h4 のスタイルをカスタマイズしている。

PDF のスタイルの変更する場合は以下を参考にする。

> ~/.gitbook/versions/3.2.3/node_modules/gitbook-plugin-theme-default/_assets/ebook/pdf.css
