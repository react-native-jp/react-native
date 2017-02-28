# react-native-jp

このリポジトリは React Native 日本語ドキュメントを管理しているレポジトリです。

## ブランチ

+ `gh-pages` 日本語ドキュメントページ
+ `gh-pages-en` 本家の英語ドキュメントページ

## ドキュメントの更新
以下のコマンドで、本家の更新を取得します。
```sh
$ git checkout gh-pages-en
$ git pull upstream gh-pages
$ git checkout gh-pages
$ git merge gh-pages-en
```

## 翻訳手順
翻訳される方は、以下の翻訳ガイドをご覧ください。  
[React Native日本語翻訳ガイド](https://github.com/react-native-jp/react-native/blob/gh-pages/CONTRIBUTING.md)
