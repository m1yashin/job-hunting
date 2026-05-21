# 02_Companies/AGENTS.md

## 目的

このフォルダは、企業ごとの作戦本部である。
企業分析、ES、素材要約、企業別面接対策を企業フォルダ内に集約する。

## 推奨構成

```text
02_Companies/
  NRI/
    企業概要.md
    企業分析.md
    素材要約.md
    面接対策.md
    ES/
      志望動機_300字.md
      ガクチカ_400字.md
```

## 配置ルール

- `02_Companies/` 直下には企業フォルダだけを作る。
- 企業ごとのESは `02_Companies/企業名/ES/` に置く。
- 企業分析は `企業分析.md` に置く。
- Webクリップや素材メモから使える情報の要約は `素材要約.md` に置く。
- 企業別の面接対策、逆質問、想定深掘りは `面接対策.md` に置く。
- 原典資料そのものは `03_メモ素材/WebClip/業界/企業/` に置く。

## 企業概要.md Properties

```yaml
---
type: company
company:
industry:
role:
priority:
status:
deadline:
next_action:
keywords: []
---
```

## ES Properties

```yaml
---
type: es
company:
question_type:
word_limit:
status:
deadline:
version:
related_answer_unit: []
---
```

## statusの使用ルール

`status` は、企業概要、ES、面接対策のように進捗判断に使うノートだけに付ける。
`企業分析.md` と `素材要約.md` は情報置き場なので、`status` を持たせず `last_reviewed` と本文チェックリストで管理する。

## statusの固定語彙

企業の `status` は以下を使う。

```text
気になる
説明会予定
説明会参加済み
ES作成中
ES提出済み
Webテスト
面接予定
結果待ち
通過
内定
落選
辞退
```

ESの `status` は以下を使う。

```text
未着手
下書き
添削中
完成
提出済み
没
```

面接対策の `status` は以下を使う。

```text
未着手
準備中
直前OK
終了
```

## 編集方針

- 面接前に企業フォルダを開けば、その企業の状況が分かる状態にする。
- ESは企業情報・素材要約・回答ユニットと接続する。
- 素材要約には原典の丸写しではなく、面接・ESで使える情報だけを書く。
- 企業固有の志望理由は `面接対策.md` とESに寄せる。
