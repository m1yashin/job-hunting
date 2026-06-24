# 03_メモ素材/AGENTS.md

## 文字コード

このファイルとこのフォルダ配下のMarkdownファイルは、文字化けを防ぐためUTF-8で開く。

## 目的

このフォルダには、まだ企業研究や選考対策に入れる前の素材メモを置く。

Web Clipperで保存した原典、ワンキャリアなどの収集メモ、Deep Researchの原稿、口コミ・OB訪問メモ、草案、ガクチカの母艦メモ、思考メモ、あとで使うかもしれない材料を扱う。

## 役割

- 原典資料はここに残し、出典つきで確認できる事実は `02_企業研究/` に反映する。
- 自分との接点、志望理由、逆質問、面接論点として使う内容は `01_選考対策/企業名/` に反映する。
- ガクチカや自己PRの母艦メモはここで育て、面接で使う形になったら `01_選考対策/共通_面接/` の該当メモに反映する。
- 口コミ・OB訪問メモは主観が混ざるため、公式情報と混ぜない。
- ここは一時置き場でもよいが、重要情報を閉じ込めたままにしない。

## 推奨構成

```text
03_メモ素材/
  WebClip/
    NRI/
      NRI_テーマ_収集.md
      NRI_選考段階_抽出質問リスト.md
    日鉄ソリューションズ/
      日鉄ソリューションズ_テーマ_収集.md
      日鉄ソリューションズ_選考段階_抽出質問リスト.md
  deep-research-report/
    企業名_テーマ_deep-research-report.md
```

口コミ_OB訪問、草案、母艦、思考メモのフォルダは、必要になった時点で作る。現時点では `WebClip/企業名/` と `deep-research-report/` を中心に運用する。

## WebClip Properties

単発のWebClipや資料メモは以下を使う。

```yaml
---
type: webclip
industry:
company:
source_type:
clip_status:
clipped:
url:
site:
title:
use_for: []
tags:
  - 就活
  - webclip
---
```

複数ページをまとめた収集メモは、既存ファイルに合わせて以下を使ってよい。

```yaml
---
type: webclip_collection
company:
source:
theme:
stage:
created:
confirmed:
target_roles: []
related_extract:
---
```

面接質問やGDテーマだけを抽出したリストは、既存ファイルに合わせて以下を使ってよい。

```yaml
---
type: question_extract
company:
stage:
source_clip:
source:
created:
target_roles: []
---
```

## 素材メモ Properties

```yaml
---
type: material_note
theme:
status:
use_for: []
related_company: []
next_action:
---
```

## clip_statusの固定語彙

```text
未読
要約済み
企業研究反映済み
選考対策反映済み
不要
```

## material_note statusの固定語彙

```text
未整理
整理中
反映済み
保留
```

## 編集方針

- 原典本文は大きく編集しない。
- 出典URLと取得日または確認日は必ず残す。
- `WebClip/` 配下は企業別フォルダに分ける。新規作成時は `WebClip/企業名/企業名_テーマ_収集.md` を基本にする。
- `deep-research-report/` はAI調査や長文調査の原稿置き場にする。事実として使う内容は `02_企業研究/`、選考で使う示唆は `01_選考対策/企業名/` に切り出す。
- 事実として使える情報は `02_企業研究/` に反映する。
- 選考で使う解釈、自分との接点、志望理由、逆質問は `01_選考対策/企業名/` に反映する。
- 反映後は `status: 反映済み`、`clip_status: 企業研究反映済み`、または `clip_status: 選考対策反映済み` にする。
- 口コミ・OB訪問メモは「仮説」「要確認」として扱い、企業研究の事実本文に混ぜない。
