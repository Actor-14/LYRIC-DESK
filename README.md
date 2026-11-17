# LYRIC DESK

歌詞制作アプリ「LYRIC DESK」の配信用リポジトリ。
Cloudflare Workers（lyricdesk）とGit連携しており、このリポジトリにファイルを push すると自動でデプロイされます。

## 更新方法
1. 新しいファイル（主に index.html）をこのリポジトリにアップロードして上書きコミット
2. 1分ほどで Cloudflare に自動デプロイ
3. アプリ側は Service Worker が新しい本体を取得します（反映されない場合はアプリを開き直す）

## 構成
- index.html … アプリ本体（単一ファイル）
- sw.js … オフライン用 Service Worker
- manifest.webmanifest … PWAマニフェスト
- 各種PNG … アイコン
- wrangler.jsonc … Cloudflare配信用設定（アプリには含めない）
