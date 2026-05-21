# 01_Selection/AGENTS.md

## 目的

このフォルダは、面接・GDの実戦準備を置く場所である。
企業固有のESや企業分析は `02_Companies/企業名/` に置き、ここには企業をまたいで使う回答力・質問・ログ・GDフレームを置く。

## 推奨構成

```text
01_Selection/
  面接/
    質問/
      00_共通質問.md
      01_SIer.md
      個別質問/
        なぜSIerなのか.md
    回答ユニット/
      研究説明.md
      ガクチカ_大学祭.md
      SIer志望理由.md
    面接ログ/
      2026-05-25_NRI_一次面接.md

  グループディスカッション/
    型/
      GD基本テンプレ.md
      GDで使える発言.md
      GD評価ポイント.md
    ログ/
      2026-05-28_日本総研_GD復習.md
```

## 配置ルール

- `01_Selection/` 直下には、原則としてAGENTS.md以外の実ノートを置かない。
- 面接の共通回答、質問、深掘り対策は `面接/` 配下に置く。
- GDの型、発言、評価観点、復習ログは `グループディスカッション/` 配下に置く。
- 企業固有の面接対策は `02_Companies/企業名/面接対策.md` に置く。
- 企業固有のESは `02_Companies/企業名/ES/` に置く。

## 選考ログProperties

```yaml
---
type: selection_log
company:
event_type:
round:
theme:
date:
result:
next_action:
score:
---
```

## event_typeの固定語彙

```text
面接
GD
説明会
Webテスト
OB訪問
面談
その他
```

## resultの固定語彙

```text
未定
通過
落選
辞退
保留
内定
```

## 編集方針

- 面接・GDは一回ごとの経験値を残す。
- 「何が起きたか」だけでなく、「次回どう変えるか」まで書く。
- 質問ノートを回答本体にしない。回答本文と深掘り対策は `面接/回答ユニット/` に置く。
- 企業別に使う内容は `02_Companies/企業名/面接対策.md` に転記する。
- 選考ログは `status` で管理せず、結果は `result`、次にやることは `next_action` で管理する。
