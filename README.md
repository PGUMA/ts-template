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
