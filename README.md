# 初期設定手順

```
yarn init
yarn add --dev typescript @types/node
yarn run tsc --init
```

※注釈

@types/node
node モジュールの型

# TSC 動作確認

```
yarn build
yarn start
```

# 変更の自動監視

[参考](https://typescript-jp.gitbook.io/deep-dive/nodejs)

```
yarn add --dev ts-node nodemon
yarn start // ファイル変更を感知してts-nodeが自動再実行されるようになる
```

# eslint の導入

```
yarn add --dev eslint @typescript-eslint/eslint-plugin @typescript-eslint/parser
touch .eslintrc.js
```

## エラーの回避

```
Parsing error: "parserOptions.project" has been set for @typescript-eslint/parser.
The file does not match your project config: .eslintrc.js.
The file must be included in at least one of the projects provided.
```

eslintrc.js が import されてないという主旨だが import 不要なので`.eslintignore`で対象外に指定する
