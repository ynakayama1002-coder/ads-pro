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
└── .cursor/skills/           … 課題提出用スキル（スライド作成など）
```

フォルダ名は回次のみ（日付は入れない）。日程が必要なら各回のメモや別表で管理する。

## 使い方

| やりたいこと | 見る場所 |
| --- | --- |
| プログラムの目的・回数 | `program.md` |
| 某回の講義内容 | `lectures/<n>/lecture-material/` |
| 某回の課題要件 | `lectures/<n>/monthly-assignment/assignment.md` |
| 課題の成果物 | `lectures/<n>/monthly-assignment/deliverables/` |
| 課題提出用スライドを作る | `.cursor/skills/slide-3pack/` |
| AI に作業させる | 先に `AGENTS.md`、必要なら `.cursor/skills/` |

## 課題提出用のスライド作成スキル

月次課題の提出スライドは、`.cursor/skills/slide-3pack/` を使う。

- **役割**: トークン対効果の3枚スライドを、統一HTMLデザインで作成する
- **起動の目安**: 「スライド作って」「3枚にまとめて」「HTMLスライド」
- **出力**: ブラウザで開ける単体 HTML（必要なら Google スライド用テキストも可）
- **置き場の例**: `lectures/<n>/monthly-assignment/deliverables/`

共通の作業ルールは [`AGENTS.md`](AGENTS.md) にあり、ツール共通。スライド作成など課題提出向けの手順だけ `.cursor/skills/` に置く。
