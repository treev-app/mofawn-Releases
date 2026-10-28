# MoFawn / Treev

コピーした日本語文章を整えたり、受信文から返信案をつくったりする、メニューバー／トレイ常駐のAI文章作成支援アプリです。

## ダウンロード

[リリースと配布状況](https://github.com/treev-app/mofawn-Releases/releases)

現在は技術検証版です。このリポジトリは非公開で、閲覧には許可されたGitHubアカウントが必要です。一般公開用のDeveloper ID署名・公証済みインストーラーはまだ提供していません。検証用のビルドはDraft Releaseで管理します。

このリポジトリは配布専用です。アプリ本体のソースコードは含めません。

- `MoFawn-*-macos-arm64-poc.zip` — Apple Silicon Mac用の開発ビルド（一般配布不可）
- 同名の`.sha256` — SHA-256チェックサム
- `release-status.json` — 現在の配布状態

## 操作方法

[操作ガイド](https://mofawn-treev.vastsloth7.chatgpt.site/guide/) / [紹介サイト](https://mofawn-treev.vastsloth7.chatgpt.site/)

1. 設定の「AI接続」で利用するAIを準備します。
2. 整えたい文章をコピーして ⌘U、または受信文をコピーして ⌘K を押します。
3. 結果を貼り付け、内容を確認してから使います。

ショートカットは変更できます。WindowsではCtrlキーを使う設計ですが、Windows実機での検証・配布はまだ行っていません。

## 現在の対応環境

- 検証ビルド：macOS / Apple Silicon（arm64）
- Apple Foundation Models：macOS 26以降、Apple Intelligence対応・有効、モデル準備完了が必要。
- Ollama：別途起動済みのローカルモデルが必要。
- クラウドAI：ユーザー自身のAPIキーを使用。実通信は検証継続中。
- 自動更新、7日間の試用、買い切り認証：未実装。

## チェックサムの確認

ZIPと同じリリースの`.sha256`を同じフォルダへ保存し、ファイル名を合わせて実行します。

```sh
shasum -a 256 -c MoFawn-0.1.0-poc.20261029-macos-arm64-poc.zip.sha256
```

チェックサム一致は配布物の同一性を確認するもので、Appleの署名・公証の代わりにはなりません。

## 問題の報告

[Issues](https://github.com/treev-app/mofawn-Releases/issues)へ、OS、バージョン、手順、機密情報を除いたエラーをお知らせください。本文やAPIキーは投稿しないでください。脆弱性の報告は[SECURITY.md](SECURITY.md)を参照してください。

Web制作データは[MoFawn Web](https://github.com/treev-app/mofawn-Web)で管理します。制作：Treev。
