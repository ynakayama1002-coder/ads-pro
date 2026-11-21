# AGENTS.md — AIエージェント共通ルール

このリポジトリで作業するAIエージェント向けの共通指示。ツール固有の設定（例: `.cursor/skills/`）より先に、ここを正とする。

## 作業前

1. `program.md` でプログラム全体の目的・回数を確認する。
2. 対象回の資料だけを読む（必要なときだけ他回を参照する）。
3. 不明点は推測で埋めず、人間に確認する。

## 情報の正本（SSoT）

| 情報 | 正本 |
| --- | --- |
| プログラム全体の目的・方針 | `program.md` |
| 講義の文字起こし | `lectures/<n>/lecture-material/transcript.md` |
| 授業内メモ | `lectures/<n>/lecture-material/class-notes.md` |
| 課題の正式要件 | `lectures/<n>/monthly-assignment/assignment.md` |
| 課題の成果物 | `lectures/<n>/monthly-assignment/deliverables/` |
| グループセッション資料 | `group-sessions/<n>/` |

同じ情報を README やメモに複製しない。案内は参照先のパスだけ書く。

## 参照ルール

- 講義の分析 → 対象回の `lecture-material/`
- 課題対応 → 対象回の `monthly-assignment/`（要件は `assignment.md`）
- グループセッション → `group-sessions/<n>/`
- 必要なファイルだけ読む（Progressive Disclosure）

## 更新ルール

- 原資料（`transcript.md`、正式な `assignment.md`、人間が書いた `class-notes.md`）は原則変更しない。
- 要約・分析・改善案など AI 生成物は、原資料と分けて `deliverables/` 等に置く。
- 既存の資料・成果物を無断で削除・上書きしない。
- AI が作った内容は、人間の確認後に確定扱いとする。

## 完了時の報告

- 変更したファイルを列挙する
- 変更理由を短く説明する
- 重複・矛盾・未確認事項があれば明示する

## Cursor 固有

月次課題向けスキルは `.cursor/skills/` にある。スキル同士をパイプライン結合しない。共通ルールは本ファイルに置き、スキル側へ重複させない。
