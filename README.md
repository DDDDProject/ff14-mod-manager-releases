# FF14 MOD Manager

Windows向けのMOD・POSE管理アプリです。
このリポジトリは配布専用です。ソースコードは公開していません。

## ダウンロード

右側の **Releases** から最新版の `FF14ModManager-バージョン-win-x64.zip` を取得してください。
GitHubが自動表示する「Source code」ではなく、アプリ名のZIPを選択してください。

ZIPをすべて展開し、`FF14ModManager.exe`を起動します。
DLLと`web`フォルダーも必要です。

## 主な機能

- MOD・POSEライブラリ、プレビュー画像、ジャンル・タグ・グループ管理。
- 対応配布サイトからのプレビュー画像取得。
- Penumbraのフォルダー構成・表示名・有効状態・優先度の確認と編集。
- テーマ、フォント、表示サイズ、多言語表示。

## 動作条件

Windows 11 x64。
.NET実行環境は同梱しています。
[Microsoft Edge WebView2 Runtime](https://developer.microsoft.com/microsoft-edge/webview2/)が必要です。
未導入の場合はMicrosoft公式サイトから導入してください。

## 更新と保存データ

アプリを終了し、新版ZIPを別フォルダーに展開して起動してください。
ライブラリは `%LOCALAPPDATA%\FF14ModManager\XmaPoc` に保存されます。
更新前にアプリ内のバックアップ機能をご利用ください。

## 問題報告

Issuesにバージョン・再現手順を記載してください。
MOD本体、個人のデータベース、ログイン情報は添付しないでください。

コード署名は付与していません。
配布ZIPのSHA-256は同じリリースの`.sha256`ファイルで確認できます。

利用条件は `TERMS.txt`、依存ソフトウェアのライセンスは配布ZIP内の `THIRD-PARTY-NOTICES.txt` と `licenses` をご確認ください。
本アプリはゲームおよび配布サイトの公式製品ではありません。
