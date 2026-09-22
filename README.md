# SUI 47 Journey - Production-style personal web app

## できること
- 47都道府県を地図風UIから選択
- 訪問済み/未訪問の管理
- 訪問日・旅メモ
- 写真・動画の保存とアルバム表示
- TODORIST（未訪問・再訪問の「行きたい/やりたい」）
- CHAPPY：旅の振り返り、Instagram、Reel構成、TikTok用文章の下書き
- JSONバックアップ/復元
- PWA対応（Web公開後、iPhoneのホーム画面に追加可能）

## 使い方
1. index.html をブラウザで開く
2. MAPから県をタップ
3. 訪問日・メモ・写真/動画・TODOを登録
4. CHAPPYでSNS用の下書きを作る
5. DATAから定期的にJSONバックアップ

## 注意
この版は「完成形の土台」として、データを端末ブラウザ内に保存します。
写真・動画を大量に扱う本番クラウド版では、認証＋クラウドストレージ＋DBを追加するのが適切です。
CHAPPYの文章生成も、現状はローカルテンプレートです。実際のChatGPT連携を入れる場合はAPIキーをブラウザへ置かず、サーバー側で安全に呼び出してください。

## Web公開
GitHub Pages、Cloudflare Pages、Vercelなどの静的ホスティングに配置できます。
PWAのservice workerはHTTPS環境で利用してください。
