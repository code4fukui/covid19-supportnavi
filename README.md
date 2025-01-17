# 新型コロナウイルス感染症　支援情報ナビ オープンソース版

## 概要

「新型コロナウイルス感染症 支援情報ナビ オープンソース版」は、行政サービス情報の詳細データを読み込ませることで簡単に支援情報ナビを作成できます。
新型コロナウイルス感染症 支援情報ナビ オープンソース版は以下の特徴があります。

* 東京都の「新型コロナウイルス感染症 支援情報ナビ」と同様に「自分にあった制度を探す」、「テーマ別に制度を見る」の機能が使用できる

* 行政サービス情報のファイルを用意することで、簡単にデータが更新できる

* ナビロジックのファイルを用意することで、簡単にロジックの更新できる

また、東京都の「新型コロナウイルス感染症 支援情報ナビ」と以下の差異があります。

* 「キーワードで検索する」機能が付属していない
* 「区市町村の関連情報を見る」機能が付属していない
* 「医療関係者向け」のメニューがない

※差異があるためPull requestをいただいても「新型コロナウイルス感染症　支援情報ナビ」に反映できない可能性があります。

より詳細な利用方法に関しては、リポジトリ内の manual.pdf をご覧ください。

## インストール

はじめに、リポジトリのファイルをすべてローカルマシンにコピーします。

Git クライアントを使用する場合は次のコマンドでコピーすることができます。

```
git clone https://github.com/code4fukui/covid19-supportnavi.git
```

つぎに依存モジュールをインストールします。

```
npm install
```

次のコマンドでサイトのファイル一式を生成することができます。
```
npm run build
```

ファイルは `dist` フォルダ内に生成されます。

## 使用方法およびカスタマイズ方法

### サービス情報の一覧の設定

manual.pdf 内の「行政サービス情報csvについて」を参照してください。

### ナビゲーションのデータ設定

manual.pdf 内の「ナビロジックcsvについて」を参照してください。

### 配色の変更

次の cssファイルを編集することにより配色を変更することができます。

- static\styles\color-def-dark.css
- static\styles\color-def-default.css
- static\styles\color-def-light.css

## 更新履歴


| 日付  | バージョン | 備考 |
| ------ | ---------------- | ---- |
| 2021-11-12 | 初版  |      |

## ライセンス

新型コロナウイルス感染症　支援情報ナビ オープンソース版は MIT ライセンスにより提供されています。ライセンスの詳細についてはライセンスドキュメント（[LICENSE.md](LICENSE.md)）を参照してください。
