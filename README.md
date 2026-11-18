# LYRIC DESK

歌詞制作アプリ「LYRIC DESK」の配信用リポジトリ。
公開は GitHub Pages（https://actor-14.github.io/LYRIC-DESK/）で行っています。

## 更新方法
1. 新しいファイル（主に index.html）をこのリポジトリにアップロードして上書きコミット
2. 1〜2分ほどで GitHub Pages に自動デプロイされます
3. アプリを開き直すと新しい版に切り替わります（反映されない場合はアプリを完全に終了してからもう一度開く）

※ GitHub Pages のキャッシュの関係で、デプロイ完了から反映まで最大10分ほどかかることがあります。

## データについて
- 歌詞・フレーズ等のデータはこのリポジトリには入っていません
- 端末内に保存されます（localStorageキー lyric-desk-v01、音源・仮歌テイクはIndexedDB）
- 定期的に設定からJSONバックアップを書き出してください

## 構成
- index.html … アプリ本体（単一ファイル）
- sw.js … オフライン用 Service Worker
- manifest.webmanifest … PWAマニフェスト
- 各種PNG … アイコン
- README.md … このファイル
- CHANGELOG.md … 更新履歴
