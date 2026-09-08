# Yurikada

**現象を説明するモデルと、そのモデルをどこまで信頼できるか検証する仕組みを、対で作ります。**

機械工学、振動・モード解析、設備診断の経験を基盤に、数値計算・統計・機械学習を独学で学び、ケーススタディと個人向けツールを作っています。このページでは、各プロジェクトの目的、試せる入口、検証の記録をまとめています。

My background is in mechanical engineering, vibration analysis, and equipment diagnostics. I am independently studying numerical methods, statistics, and machine learning through reproducible case studies and personal tools.

## まず見るプロジェクト

| プロジェクト | 確認できること | 入口 |
|---|---|---|
| [mech-design-study](https://github.com/Yurikada/mech-design-study) | 梁の応力・熱・振動、設計案比較、梁FEMと解析解の照合。未評価の設計分野も表示 | [図付き講義](https://github.com/Yurikada/mech-design-study/blob/main/docs/learning/01-lecture.md) |
| [modal-analysis-portfolio](https://github.com/Yurikada/modal-analysis-portfolio) | LSCF・CMIF・共有ポールMIMOフィッティングを正解値付き合成データで検証 | [Streamlitアプリ](https://modal-analysis-portfolio-af6875oymekgugugcy7tsx.streamlit.app/) |
| [bearing-diagnostics](https://github.com/Yurikada/bearing-diagnostics) | CWRUでの手法照合、NASA IMSの劣化検出、独立runへの転移と限界 | [ケーススタディ](https://yurikada.github.io/bearing-diagnostics/) |
| [agent-viz](https://github.com/Yurikada/agent-viz) | MLflowの試行台帳、ケース別比較、判断の根拠、人間とエージェントの双方向パネル | [合成データで試す](https://github.com/Yurikada/agent-viz#使い方) |
| [kaggle-house-prices-workflow](https://github.com/Yurikada/kaggle-house-prices-workflow) | 外れ値の扱いとモデル選択を同じ比較条件で検討した実験 | [公開コードと実験表](https://github.com/Yurikada/kaggle-house-prices-workflow#公開されている内容) |
| [kaggle-store-sales-workflow](https://github.com/Yurikada/kaggle-store-sales-workflow) | 16日ブロック予測の時系列CV、特徴比較、CV改善と公開スコアの食い違い | [検証設計と結果](https://github.com/Yurikada/kaggle-store-sales-workflow) |

各リポジトリは個人開発・学習の成果物です。実装の動作確認、本人の理解、実設備や別データへの一般化は、それぞれ分けて扱います。AI支援による実装・整理も利用し、独力実装や業務での導入実績と混同しないようにしています。

## ブラウザで試す・読む

セットアップなしで見られる入口です。Streamlitは休止後に起動待ちになる場合があります。

| デモ・レポート | 内容 |
|---|---|
| [Modal Analysis](https://modal-analysis-portfolio-af6875oymekgugugcy7tsx.streamlit.app/) | 合成FRFからモードを同定する解析アプリ |
| [Bearing Diagnostics](https://yurikada.github.io/bearing-diagnostics/) | 振動診断の結果・条件・転移の限界 |
| [Bayesian Optimization](https://yurikada.github.io/bayesopt-process/) | 少量実験、獲得関数、ノイズ、較正のケーススタディ |
| [Geospatial Change Detection](https://yurikada.github.io/geo-change-detection/) | Sentinel-2による山火事変化検出と参照データとの照合 |
| [Similarity Radar](https://yurikada.github.io/similarity-radar/) | 合成データで高次元類似度の投影・距離・密度を探索 |
| [SceneLex](https://yurikada.github.io/scenelex/) | 英単語と画像を結びつけるクイズ |
| [Math Painting](https://yurikada.github.io/math-painting/) | 複素平面の写像を使った画像変形とPNG出力 |

## 公開プロジェクト一覧

プロフィール用の本リポジトリを除く18件を、用途別に整理しています。

### 機械工学・数値計算・センシング

| リポジトリ | 内容 |
|---|---|
| [mech-design-study](https://github.com/Yurikada/mech-design-study) | 個別の設計技術と制約の統合を、解析解・比較CLI・梁FEMで学ぶ |
| [modal-analysis-portfolio](https://github.com/Yurikada/modal-analysis-portfolio) | 実験モード解析のPythonコアとStreamlit UI |
| [bearing-diagnostics](https://github.com/Yurikada/bearing-diagnostics) | 信号処理の数値照合から軸受の劣化検出まで |
| [bayesopt-process](https://github.com/Yurikada/bayesopt-process) | NumPyによるガウス過程・獲得関数の実装と比較検証 |
| [geo-change-detection](https://github.com/Yurikada/geo-change-detection) | 衛星画像の変化検出、評価指標、参照定義の比較 |

### データ分析・実験管理

| リポジトリ | 内容 |
|---|---|
| [agent-viz](https://github.com/Yurikada/agent-viz) | 試行・ケース・判断の根拠を共有する可視化基盤 |
| [kaggle-titanic-experiment-management](https://github.com/Yurikada/kaggle-titanic-experiment-management) | 事前登録した比較、誤りの層別、不確実性の学習記録 |
| [kaggle-house-prices-workflow](https://github.com/Yurikada/kaggle-house-prices-workflow) | 外れ値処理とnested CVによるモデル比較 |
| [kaggle-store-sales-workflow](https://github.com/Yurikada/kaggle-store-sales-workflow) | 時系列の検証分割と16日先までの予測実験 |
| [similarity-radar](https://github.com/Yurikada/similarity-radar) | 次元削減・回転不変な読み取り・密度・時系列整列 |

### 学習・日常のツール

| リポジトリ | 内容 |
|---|---|
| [enja-reader](https://github.com/Yurikada/enja-reader) | 文単位で日英を切り替えるHTML生成ツールとChrome拡張 |
| [scenelex](https://github.com/Yurikada/scenelex) | Wikimedia Commonsの画像を使った英語語彙学習 |
| [ai-english-conversation-tutor](https://github.com/Yurikada/ai-english-conversation-tutor) | 音声認識、文法フィードバック、読み上げを備えた英会話練習 |
| [kajiflow](https://github.com/Yurikada/kajiflow) | 「今の1件」を提示する家事管理とタスク・購買記録の連携 |
| [math-painting](https://github.com/Yurikada/math-painting) | ビルド不要のCanvas画像変形スタジオ |
| [forza-horizon-telemetry-monitor](https://github.com/Yurikada/forza-horizon-telemetry-monitor) | UDPテレメトリから走行差分や運転フィードバックを表示 |

### 取引記録・スクリーニングの検証

| リポジトリ | 内容 |
|---|---|
| [trade-statistics](https://github.com/Yurikada/trade-statistics) | 取引履歴を分析するレビュー用パイプライン。合成データの実行例付き |
| [jp-stock-screener](https://github.com/Yurikada/jp-stock-screener) | ルールによる銘柄抽出と、抽出後リターンの追跡・検証 |

## 進め方

- 変更前に仮説と比較条件を置く
- 指標を参照定義、分母、測定限界とセットで読む
- 計算の実装は手計算または確立ライブラリと照合する
- 予測を外した場合も、原因と訂正を記録する
- 実装済み、推論、未検証を分けて説明する

## Profiles

- [Kaggle: yosukeinada](https://www.kaggle.com/yosukeinada)
