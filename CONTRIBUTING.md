# React Native 日本語翻訳ガイド

翻訳プロジェクトに貢献したい方は以下の内容を一読のうえ、翻訳をお願いします。


## 貢献方法

1. このレポジトリをフォークします
2. `gh-pages` ブランチからトピックブランチを作成します
3. 変更をコミットします
4. フォークした自分のレポジトリに Push します
5. 問題がなければ、プルリクエストを `react-native-jp/react-native` の `gh-pages` ブランチに送ります

## 翻訳のゆらぎ & トーン

### 文体
「だである」ではなく「ですます」調

> React Native lets you build mobile apps using only JavaScript.

- NG : React Nativeでは、JavaScriptのみを使用してモバイルアプリを構築できる。
- OK : React Nativeでは、JavaScriptのみを使用してモバイルアプリを構築できます。

### 原則、一語一句翻訳。ただし日本語として分かりにくい場合は読みやすさを優先

> It uses the same design as React, letting you compose a rich mobile UI from declarative components.

- NG: これはReactと同じデザインを使用しており、宣言的なコンポーネントから豊富なモバイルUIを作成できます。
- OK: これはReactと同じシンタックスを使用しており、宣言的なコンポーネントから豊富なモバイルUIを作成できます。

### 原文に使われる ':' や '!' や '?' などの記号は極力残して翻訳

> Example:

- NG: 例
- OK: 例:

ただし、文の途中にハイフン`-` や セミコロン`;` など、その記号があると理解しづらい訳になる場合は、削除をお願いします。

### 単語の統一 (特に技術用語)

- 技術用語は原則英語、ただし日本語で一般的に使われている場合は日本語で問題ありません。
  - 例: 英語の filter 、日本語のフィルタ
- 和訳に困った場合や和訳にして分かりづらい場合は、翻訳文と英語(翻訳文に括弧付け)でお願いします。
  - 例: components -> components (コンポーネント)
