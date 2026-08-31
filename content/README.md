# コンテンツ一覧

このフォルダーには、ブラウザだけで動く JupyterLite サイトのノートブックとデータが入っています。
ファイルブラウザからノートブックをダブルクリックして開き、上から順にセルを実行してください。
(Python の初回起動と、一部ノートブックの先頭セルは数十秒かかることがあります)

## tutorials/ — チュートリアル

| ファイル | 説明 |
|---|---|
| `python-tutorial.ipynb` | Python 入門。変数・条件分岐・ループ・関数などの基本文法を初心者向けに解説 |
| `javascript-tutorial.ipynb` | JavaScript 入門。JS カーネルで基本文法を学ぶ |
| `p5-tutorial.ipynb` | p5.js 入門。図形描画やアニメーションなどクリエイティブコーディングの基礎 |
| `plotnine-tutorial.ipynb` | plotnine 入門。R の ggplot2 と同じ「グラフィックスの文法」で Python のグラフを描く |
| `neural-network-tutorial.ipynb` | ニューラルネットワーク入門。NumPy だけで順伝播・逆伝播を実装し、手書き数字を分類する |
| `pandas-crosstab.ipynb` | pandas のクロス集計演習。`pd.crosstab()` の使い方を課題形式で練習する |

## statistics/ — 統計

| ファイル | 説明 |
|---|---|
| `statistics-python.ipynb` | 統計分析 中級編(Python)。記述統計から検定・回帰・時系列まで 48 例題 + 練習問題 |
| `statistics-javascript.ipynb` | 統計分析(JavaScript)。ライブラリなしの純 JS で分布や検定を実装する 39 例題 |
| `hypothesis-test-exercises.ipynb` | 仮説検定の練習問題集。t 検定・F 検定・分散分析・回帰分析・比率の検定・カイ二乗検定を例題 1 問 + 練習 11 問で練習 |

## projects/ — 分析プロジェクト

| ファイル | 説明 |
|---|---|
| `weather-hypothesis.ipynb` | 仮説検証プロジェクト(フル版)。ダミー天気データを生成し、5 つのモデル比較・32 パターン分析・Permutation Importance・ブートストラップ信頼区間まで行う |
| `weather-hypothesis-basic.ipynb` | 同プロジェクトの入門版。データ作成 → 時系列分割 → 学習 → 評価という仮説検証の基本の流れを最小限の道具で体験する |

## games/ — p5.js ゲーム

| ファイル | 説明 |
|---|---|
| `p5-game-catch.ipynb` | 落ちてくるアイテムをキャッチするゲーム |
| `p5-game-breakout.ipynb` | ブロック崩し |
| `p5-game-snake.ipynb` | スネークゲーム |
| `p5-game-flappy.ipynb` | 障害物の隙間を飛び抜けるフラッピー風ゲーム |
| `p5-game-whack.ipynb` | もぐらたたき |

## examples/ — 各カーネルの最小デモ

| ファイル | 説明 |
|---|---|
| `python.ipynb` | Python(Pyodide)カーネルの基本デモ |
| `javascript.ipynb` | JavaScript カーネルの基本デモ |
| `p5.ipynb` | p5.js カーネルの基本デモ |

## pyodide/ — Python ライブラリのデモ

| ファイル | 説明 |
|---|---|
| `matplotlib.ipynb` | matplotlib によるグラフ描画 |
| `plotly.ipynb` | Plotly によるインタラクティブなグラフ |
| `altair.ipynb` | Altair(Vega-Lite)による宣言的な可視化 |
| `folium.ipynb` | Folium による地図表示 |
| `ipyleaflet.ipynb` | ipyleaflet によるインタラクティブな地図 |
| `ipycanvas.ipynb` | ipycanvas によるキャンバス描画 |
| `interactive-widgets.ipynb` | ipywidgets によるスライダーなどの対話的ウィジェット |
| `renderers.ipynb` | 各種 MIME レンダラー(Vega・GeoJSON・FASTA など)の表示デモ |
| `pyb2d/` | 物理エンジン pyb2d のデモ集(チュートリアル、ニュートンのゆりかご、ガウスの板など)と `pyb2d/games/` のミニゲーム 4 本 |

## data/ — ノートブックが使うデータ

| ファイル | 説明 |
|---|---|
| `iris.csv` | アヤメの計測データ 150 件。2 行目にわざと表記の傷(`se`)があり、データクリーニングの練習に使う |
| `bar.vl.json` | Vega-Lite の棒グラフ定義(レンダラーのデモ用) |
| `Museums_in_DC.geojson` | ワシントン D.C. の博物館の位置データ(GeoJSON 表示のデモ用) |
| `fasta-example.fasta` | 塩基配列のサンプル(FASTA レンダラーのデモ用) |
| `matplotlib.png` | 画像表示のサンプル |

> **メモ**: ノートブックへの変更はブラウザ内(IndexedDB)に保存され、サイト本体は変わりません。
> 元の状態に戻したいときは、ファイルを削除してページを再読み込みしてください。
