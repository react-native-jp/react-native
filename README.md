# react-native-jp

このリポジトリは React Native 日本語ドキュメントを管理しているレポジトリです。

## ブランチ

+ `gh-pages` 日本語ドキュメントページ
+ `gh-pages-en` 本家の英語ドキュメントページ

## 手順

以下のコマンドで、本家の更新を取得します。
```sh
$ git checkout gh-pages-en
$ git pull upstream gh-pages
$ git checkout gh-pages
$ git merge gh-pages-en
```

変更あった箇所を変更し、pushします。
```sh
$ vim example.html
$ git push origin gh-pages
```
