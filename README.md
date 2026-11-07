# 返礼品・年間カレンダージェネレーター

GitHub Pages 用の静的サイトです。ビルド不要です。

## 公開手順

1. GitHubで新しいリポジトリを作成します（例: `calendar-generator`）。
2. `index.html` と `.nojekyll` をリポジトリの**ルート**にアップロードします。
3. リポジトリの **Settings → Pages → Build and deployment** で **Deploy from a branch** を選択します。
4. **Branch: `main` / Folder: `/(root)`** を選び、**Save** します。
5. デプロイ後、`https://<GitHubユーザー名>.github.io/calendar-generator/` にアクセスします。

## 機能

- 1年12ヶ月を一覧表示
- 左側の操作ペインから各月の画像を選択
- 各月の画像のズーム・左右上下位置調整、プレビュー上のドラッグ操作
- `japan-holidays` の年別JSONを取得して日本の祝日を表示
- 月別1600×1000px PNGを12枚ZIP出力

## 注意

- カレンダーで選択した画像はブラウザ内で処理され、GitHub Pagesや外部サイトにアップロードされません。
- 祝日データは外部サイト `https://mati0516.github.io/japan-holidays/` にアクセスして取得します。取得できなければZIP出力は無効になります。
- 画像選択内容と調整値はページ更新で失われます。
- GitHub Pagesで公開したページはインターネット上からアクセス可能です。
