# CLAUDE.md テンプレート（特典6）

# （プロジェクト名）— Claude Code への指示

作業の前に、必ず次を読むこと。
- docs/spec.md（要件・受け入れ基準・状態）
- docs/decisions.md（決定と理由）
- docs/open-questions.md（未確定事項）

## コマンド
- ビルド：（例：npm run build）
- 単体試験：（例：npm test）
- 画面試験：（例：npm run e2e）
- 秘密情報の検査：（例：npm run check）

## 構成
- 編集するもの：（例：src/）
- 生成物（直接編集しない）：（例：index.html）
- 秘密情報（コミットしない）：（例：config.js）

## ルール
1. 仕様を変えるときは、先に docs/spec.md を更新する
2. 実装とテストに、要件の番号（FR・NFR・AC）を書く
3. 判断を変えたら docs/decisions.md に追記する（既存は消さず「置き換え」と書く）
4. 未確定の値は推測で確定させず、docs/open-questions.md に書く
5. APIキーを、ソースや画面に書かない
6. 完了の報告は、関係する AC の合否を番号ごとに書く

## 完了の定義
- 検証（ビルド・試験・検査）が通る
- 変更したロジックに試験がある
- 生成物が最新
- 仕様の状態と未確定事項が更新されている

## 読み取りの禁止（.claude/settings.json で設定）
- 秘密情報のファイル（例：config.real.js）
- 試験の結果フォルダ（例：test/results/）
