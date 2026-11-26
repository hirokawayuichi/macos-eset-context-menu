# macos-eset-context-menu
ESET Endpoint Security / Endpoint Antivirus / Cyber Security for macOS でファイルを検査するための、非公式の Finder コンテキストメニュー(クイックアクション)です。

## 動作環境
- Apple macOS
- 次のいずれかの ESET 製品
  - ESET Endpoint Security
  - ESET Endpoint Antivirus
  - ESET Cyber Security

## インストール
1. 使いたいワークフローをダウンロードします。
   - `EsetScan.workflow`: 検査結果をダイアログで表示します。
   - `EsetScanTerm.workflow`: ターミナルを開いて検査結果を表示します。
2. ダウンロードした `.workflow.zip` ファイルをダブルクリックして展開します。
3. `.workflow` ファイルをダブルクリックし、**インストール** をクリックします。
4. Finder でファイルまたはフォルダを選択して右クリックし、**クイックアクション** → **EsetScan**(または **EsetScanTerm**)を選びます。

macOS にワークフローがブロックされた場合は、ターミナルで次のコマンドを実行してから、もう一度お試しください。

```zsh
xattr -dr com.apple.quarantine ~/Downloads/EsetScan*.workflow
```

## アンインストール
`~/Library/Services` からワークフローを削除します。

## 免責事項
本ツールは非公式のツールであり、ESET 社および Anthropic 社とは関係ありません。ご利用は自己責任でお願いします。

## クレジット
- 設計:Y.H.
- 実装:Anthropic の Claude(Opus 5.5)を使用して作成
