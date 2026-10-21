# FF14 MOD Manager

Windows向けのMOD・POSE管理アプリです。
このリポジトリは配布専用です。ソースコードは公開していません。

## ダウンロード

**標準は軽量版です。**
[最新版のダウンロードページ](https://github.com/DDDDProject/ff14-mod-manager-releases/releases/latest)から、`FF14ModManager-バージョン-win-x64-lite.zip` を取得してください。
GitHubが自動表示する「Source code」ではなく、アプリ名のZIPを選択してください。

ZIPをすべて展開し、`FF14ModManager.exe`を起動します。
DLLと`web`フォルダーも必要です。

## 主な機能

- MOD・POSEライブラリ、プレビュー画像、ジャンル・タグ・グループ管理。
- 対応配布サイトからのプレビュー画像取得。
- Penumbraのフォルダー構成・表示名・有効状態・優先度の確認と編集。
- テーマ、フォント、表示サイズ、多言語表示。

## 初回起動に必要なもの

Windows 11 x64。

軽量版は、次の2つを使用します。
すでにインストールされていれば、再導入は不要です。

| 必要な実行環境 | 導入方法 |
|---|---|
| **.NET 10 Desktop Runtime・Windows x64** | [Microsoft公式ダウンロード](https://dotnet.microsoft.com/download/dotnet/10.0)で「.NET Desktop Runtime」のWindows **x64**を選び、インストールしてください。 |
| **Microsoft Edge WebView2 Runtime** | [Microsoft公式ダウンロード](https://developer.microsoft.com/microsoft-edge/webview2/)の「Evergreen Standalone Installer」で **x64**を選び、未導入の場合にインストールしてください。 |

**.NETは「Desktop Runtime」を選んでください。**
ASP.NET Core Runtimeや、名称が「.NET Runtime」のものだけでは画面を起動できません。
開発用のSDKは不要です。

1. 上記の実行環境をインストールします。
2. 軽量版ZIPを「すべて展開」します。
3. 展開したフォルダー内の`FF14ModManager.exe`を起動します。

ファイル名に`-lite`のない通常版は.NET実行環境を同梱しています。
ダウンロードサイズは大きくなりますが、アプリの機能は同じです。
通常版でもWebView2 Runtimeは必要です。
軽量版と通常版を同時に起動しないでください。

## 更新と保存データ

アプリを終了し、新版ZIPを別フォルダーに展開して起動してください。
ライブラリは `%LOCALAPPDATA%\FF14ModManager\XmaPoc` に保存されます。
更新前にアプリ内のバックアップ機能をご利用ください。

## 問題報告

Issuesにバージョン・再現手順を記載してください。
MOD本体、個人のデータベース、ログイン情報は添付しないでください。

コード署名は付与していません。
初回起動時にMicrosoft Defender SmartScreenの警告が出る場合があります。
発行元の利用実績を評価する仕組みのため、未署名の配布版で警告の非表示を保証することはできません。
配布ZIPのSHA-256は同じリリースの`.sha256`ファイルで確認できます。

利用条件は `TERMS.txt`、依存ソフトウェアのライセンスは配布ZIP内の `THIRD-PARTY-NOTICES.txt` と `licenses` をご確認ください。
本アプリはゲームおよび配布サイトの公式製品ではありません。
