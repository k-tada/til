### GitのPre-XXX Hookを簡単に追加する

https://github.com/typicode/husky を利用する

# 使い方
## インストール
```いつもの
yarn add -D husky
```

## 設定
`package.json`に以下のような感じでhookを埋め込むだけ

```json:package.json
  "scripts": {
    "precommit": "`npm bin`/eslint ./src && npm run stylelint",
    "prepush": "npm run test"
  }
```

