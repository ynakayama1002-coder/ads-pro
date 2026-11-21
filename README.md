# ads-pro

ADS Pro（AI-Driven School Pro）の教材・課題・成果物・Agent スキルを置くリポジトリ。

## 目的

講義と課題の正本を一箇所に集め、人間と AI が迷わず参照できるようにする。プログラム全体の方針は [`program.md`](program.md)、AI 向け共通ルールは [`AGENTS.md`](AGENTS.md)。

## ディレクトリ構成

```text
ads-pro/
├── README.md                 … 人間向け案内（本ファイル）
├── AGENTS.md                 … AI 共通ルール
├── program.md                … プログラム全体の正本
├── lectures/                 … 講義 1st〜13th
│   └── <n>/
│       ├── lecture-material/ … transcript.md / class-notes.md / 配布資料
│       └── monthly-assignment/
│           ├── assignment.md
│           └── deliverables/ … 提出物（ある回のみ）
├── group-sessions/           … グループセッション 1st〜6th
│   └── <n>/
│       ├── lecture-material/
│       └── technical-assignment/
└── .cursor/skills/           … Cursor 固有スキル
```

フォルダ名は回次のみ（日付は入れない）。日程が必要なら各回のメモや別表で管理する。

## 使い方

| やりたいこと | 見る場所 |
| --- | --- |
| プログラムの目的・回数 | `program.md` |
| 某回の講義内容 | `lectures/<n>/lecture-material/` |
| 某回の課題要件 | `lectures/<n>/monthly-assignment/assignment.md` |
| 課題の成果物 | `lectures/<n>/monthly-assignment/deliverables/` |
| AI に作業させる | 先に `AGENTS.md`、必要なら `.cursor/skills/` |

## AI ツールについて

共通ルールは `AGENTS.md` に集約している（Cursor / 他ツール共通）。Cursor 専用のスキルだけ `.cursor/skills/` に置く。
