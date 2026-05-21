# 03_メモ素材/AGENTS.md

## 目的

このフォルダには、まだ企業フォルダやSelectionに入れる前の素材メモを置く。
Web Clipperで保存した原典、草案、ガクチカの母艦メモ、思考メモ、あとで使うかもしれない材料を扱う。

## 役割

- 原典資料はここに残し、企業ごとに使える要約は `02_Companies/企業名/素材要約.md` に転記する。
- ガクチカや自己PRの母艦メモはここで育て、面接で使う形になったら `01_Selection/面接/回答ユニット/` に反映する。
- 企業固有の情報は、整理できた段階で `02_Companies/企業名/` に移す。
- ここは一時置き場でもよいが、重要情報を閉じ込めたままにしない。

## 推奨構成

```text
03_メモ素材/
  WebClip/
    業界/企業/YYYY-MM-DD_資料名.md
  草案/
    志望動機_断片.md
    逆質問メモ.md
  母艦/
    ガクチカ_大学祭_母艦.md
    研究説明_母艦.md
  思考メモ/
    迷っていること.md
```

## WebClip Properties

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

## 素材メモProperties

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
企業フォルダ反映済み
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
- 使える情報は `02_Companies/企業名/素材要約.md`、`02_Companies/企業名/企業分析.md`、または `01_Selection/面接/回答ユニット/` に反映する。
- 反映後は `status: 反映済み` または `clip_status: 企業フォルダ反映済み` にする。
- 出典URLと取得日は必ず残す。
