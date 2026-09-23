BTCサイクル比較 v3.0 full-cycle

目的
- 2010年7月の市場価格データ開始から現在まで、BTCの主要サイクルを同じ軸で比較する。
- 主要サイクル：2011、2013前半、2013後半、2017、2021、現在。
- 比較モード：ATH→現在 / ATH→底値 / 底値前後 / ATH→次ATH。

データ
- 2010-07-18〜2017-08-16：CoinGecko由来の日次BTC/USD履歴（GitHub公開ミラー、jsDelivrフォールバック）。
- 2017-08-17以降：Binance Spot API BTCUSDT daily klines。
- APIキー不要。
- 取得データはlocalStorageに保存。古い履歴は保存済みデータを再利用する。

UI / 動作
- PC / iPhone / Androidのレスポンシブ対応。
- 更新ボタン押下中は「取得中」と表示し二重押しを防止。
- PWA対応。ホーム画面追加可能。

GitHub Pages反映
1. index.html
2. manifest.webmanifest
3. sw.js
4. README_iPhone_API.txt
をGitHubへ上書きアップロードする。

注意
- Bitcoinネットワーク自体は2009年開始だが、市場価格比較は2010年7月以降を対象とする。
- 2017年8月付近でデータソースが切り替わるため、価格定義に小さな差があり得る。
- 現在サイクルの底値は未確定のため「暫定底」と表示。
- このアプリは位置確認用。売買判断ではない。
