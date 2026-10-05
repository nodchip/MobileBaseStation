# 異世界基地局（仮称）

『異世界転生した通信インフラ技術者、チート能力が「移動基地局車召喚」でした ～圏外の辺境から世界をつなぎます～』の執筆用リポジトリ。

## ファイル構成

```text
MobileBaseStation/
├── README.md                         構成・作業の入口
├── AGENTS.md                         この作品での執筆ルール
├── .agents/skills/episode-review-fix-loop/
│   └── SKILL.md                      Lunaによる二段階レビュー
├── manuscript/
│   ├── PPPP-episode-NN.txt           各話本文の唯一の正本（執筆時に作成）
│   └── PPPP-interlude-chapter-NN.txt 章末幕間の正本（作成時に追加）
├── planning/
│   ├── source-request.txt            提示された依頼・設定の原文控え
│   ├── concept.md                    作品の核・テーマ
│   ├── characters.md                 人物設定
│   ├── world.md                      世界・勢力・能力・通信仕様・用語
│   ├── outline.md                    全章構成案・日常回の題材
│   ├── chapter-01.md                 第1章の詳細設計・地理・運用案
│   ├── chapter-02.md                 第2章の詳細プロット・仮の地理と運用案
│   ├── open-questions.md             未決事項と採用した判断
│   ├── continuity.md                本文で確定した時系列・設備・伏線
│   ├── progress.md                  話数・章・タイトル・執筆／投稿状況
│   ├── episode-NN.md                各話のプロット（具体化時に作成）
│   └── reviews/
│       └── NN.md                    レビュー記録（実施時に作成）
└── publishing/
    ├── work.md                      作品名・紹介文・タグなど
    ├── format.md                    本文と投稿の書式
    └── checklist.md                 各話の投稿前後チェック
```

`NN` は章をまたぐ通し話数（01、02、…、99、100、…）、`PPPP` は幕間も含めた4桁の投稿順。章別フォルダには分けず、章との対応を progress.md に記録する。ファイル名の昇順が投稿順になる。

本文ファイルの文頭には `第N話『話タイトル』` を置き、空行を1行挟んで物語を始める。話数・話タイトルは progress.md と一致させ、公開URLも同資料で管理する。詳細な書式は publishing/format.md に従う。publishing/ に本文の複製を置かないことで、修正漏れを防ぐ。未執筆の空本文や架空のレビュー記録は作成しない。

## 資料の扱い

各章の詳細プロット（planning/chapter-NN.md）の先頭見出しは `# 第N章『章タイトル』` とする。Nはゼロ埋めしない半角数字とし、見出し末尾に「詳細プロット」は付けない。例：`# 第1章『圏外の村』`。

source-request.txt は原文控えとして保存する。現在の設定は concept.md・characters.md・world.md、構成案は outline.md に整理した。後から採用した変更は該当資料と open-questions.md の決定履歴に記録する。未決事項は本文執筆時に必要な範囲から解決し、提案を確定設定と混同しない。

## 執筆から投稿まで

1. 設定・構成・直前までの本文・継続性を読み、episode-NN.md にその話の出来事と到達点を具体化する。
2. manuscript/PPPP-episode-NN.txt を執筆し、プロジェクト内の episode-review-fix-loop に従ってレビューと修正を行う。PPPP は4桁の投稿順で、幕間にも付ける。
3. 確定した出来事を continuity.md、執筆状況とレビュー記録へのリンクを progress.md に反映する。
4. 投稿依頼があれば checklist.md に沿って投稿画面とプレビューを確認し、投稿後に公開状況を記録する。

第1章は第1〜12話の物語編と、統也が記した話数のない幕間「三日分の日報」で構成する。章全体の設計は [planning/chapter-01.md](planning/chapter-01.md)、各話は planning/episode-01.md〜episode-12.md、幕間の正本は [manuscript/0013-interlude-chapter-01.txt](manuscript/0013-interlude-chapter-01.txt) を参照する。第1〜12話の本文・二段階レビューは完了。幕間の二段階レビューも完了。第2章は[章全体の詳細プロット](planning/chapter-02.md)と第13〜24話の各話プロットを作成済み。第13〜20話の本文・レビューは完了し、第21〜24話は未着手。カクヨム投稿は未着手。最新状況は planning/progress.md を参照する。

## スキルの取り込み元

`C:\home\nodchip\akai-kitsune-midori-tanuki\.agents\skills\episode-review-fix-loop\SKILL.md` を2026-09-16に取り込み、本作の人物・通信技術・テーマに合わせて確認項目を変更した。二段階レビュー、毎周回の新規Luna、全重要度の指摘解消、本文のSHA-256照合は維持している。
