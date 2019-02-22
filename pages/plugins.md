# プラグイン

ここでは、おすすめのプラグインについて記載する。今回利用する expandable-chapters プラグインは子メニューを開閉するためのプラグイン。

`book.json` にインストールするプラグインを追記する。

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
