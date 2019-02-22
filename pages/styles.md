# スタイル

ここでは、HTML と PDF のスタイルをカスタマイズする方法にについて記載する。

`book.json` の `styles` に指定した css でスタイルを上書きする。

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

今回は主にメニューや `h2`, `h4` のスタイルをカスタマイズしている。PDF のスタイルをカスタマイズする場合、クラス指定が HTML と異なることがあるため、デフォルトのスタイルを参考にする。

> ~/.gitbook/versions/3.2.3/node_modules/gitbook-plugin-theme-default/_assets/ebook/pdf.css
