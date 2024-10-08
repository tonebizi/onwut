## onwut

`onwut` は、経済産業省のウェブサイトからPDFレポートをスクレイピングし、特定の条件に基づいて処理するためのPythonライブラリです。このライブラリは、データ分析や経済研究に役立ちます。

## 特徴
- **自動スクレイピング**: 経済産業省の公開データからPDFレポートを自動的に取得。
- **柔軟な検索機能**: 特定の期間やキーワードに基づいてレポートを検索・フィルタリング。
- **簡単なインストール**: Python環境で簡単にインストール可能。

## インストール
`onwut` をインストールするには、以下のコマンドを使用します。

```bash
pip install onwut
```

## 使い方
基本的な使い方は以下の通りです。指定した期間に「産業」というキーワードを含むレポートを検索します。
```python
import onwut.main as onwut_main

# 例: 2024年1月から2024年12月までの期間に該当するすべてのレポートを検索
onwut_main.main(start_date="2024-01", end_date="2024-12", scrape=True)

```

```python
import onwut.main as onwut_main

# 例: 2024年1月から2024年12月までの期間に「産業」というキーワードを含むレポートを検索
onwut_main.main(start_date="2024-01", end_date="2024-12", search_string="産業", scrape=True)

```
## 出力例
```
タイトル: 鉱工業生産
日付: 2024-01
URL: https://www.meti.go.jp/statistics/tyo/iip/reference/b202401.pdf
内容: 鉱工業生産は前年同月比で増加...
```
## 貢献
このプロジェクトはオープンソースであり、コミュニティの皆様の貢献を歓迎しています。バグ修正、新機能の提案、ドキュメントの改善など、どのような貢献でも大歓迎です。
特に、現在 onwut は経済産業省のドキュメントに焦点を当てていますが、その他の政府機関のドキュメントを取得する機能を追加することを目指しています。例えば、総務省、厚生労働省、財務省などのドキュメントも自動で取得できるようにするための貢献を歓迎します。


