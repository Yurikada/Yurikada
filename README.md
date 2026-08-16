# Yurikada

**現象を説明するモデルと、そのモデルをどこまで信頼できるか検証する仕組みを、対で作ります。**

*I build models of real-world phenomena together with checks that make their evidence and limits explicit.*

機械工学、振動・モード解析、設備診断の経験を基盤に、数値計算、統計、機械学習を用いた検証可能な成果物を作っています。結果だけでなく、比較条件、評価基準、外した予測、残る限界まで記録することを重視しています。

My background is in mechanical engineering, vibration analysis, and equipment diagnostics. I build reproducible numerical and machine-learning case studies, with explicit baselines, validation criteria, failed predictions, and limitations.

## Try the live demos

| Project | What you can inspect | Demo |
|---|---|---|
| SceneLex | An image-first English vocabulary interface | [Open app](https://yurikada.github.io/scenelex/) |
| Math Painting | Interactive complex-function visualization | [Open app](https://yurikada.github.io/math-painting/) |
| Modal Analysis Portfolio | LSCF / CMIF / MIMO modal-analysis workflow with synthetic data | [Open Streamlit app](https://modal-analysis-portfolio-af6875oymekgugugcy7tsx.streamlit.app/) |
| Bearing Diagnostics | Reproducible bearing-fault case study and evidence boundaries | [Open case study](https://yurikada.github.io/bearing-diagnostics/) |
| Bayesian Optimization | Staged experiments, calibration, and limitations | [Open case study](https://yurikada.github.io/bayesopt-process/) |
| Geospatial Change Detection | Wildfire change detection evaluated against reference data | [Open case study](https://yurikada.github.io/geo-change-detection/) |
| Similarity Radar | Rotation-invariant similarity landscapes read by distance and density | [Open demo](https://yurikada.github.io/similarity-radar/) |

The Streamlit demo may need to be woken after inactivity. Each case study states
what is implemented, what was validated, and what remains unverified.

## Representative work

### [bearing-diagnostics](https://github.com/Yurikada/bearing-diagnostics)

転がり軸受の振動診断ケーススタディです。FFT・Welch PSD・Hilbertエンベロープ解析を自前実装してscipyと照合し、正解既知のCWRUデータで手法を固定してから、NASA IMSのrun-to-failureデータに適用しました。故障特徴周波数はデータを見る前に幾何と回転数から宣言し、検出リードタイムと誤報の評価、独立runへの転移テスト、残る限界の開示までをレポートにまとめています。

*A rolling-bearing vibration-diagnostics case study: signal-processing core implemented from scratch and validated against scipy, methods frozen on labeled CWRU data, then applied to NASA IMS run-to-failure detection — including a transfer test on an independent run and explicit limitations.*

### [similarity-radar](https://github.com/Yurikada/similarity-radar)

高次元類似度の2D投影を「軸ではなく距離と密度で読む」ための可視化研究です。回転不変な読み取り、密度面、クラスタリング、時系列トレンドまでの6段パイプラインを実装し、2Dで立てた仮説を高次元側で検証する往復を、2つのドメインのケーススタディで記録しています。公開デモは合成データのみで動作します。

*A landscape-visualization study of high-dimensional similarity: rotation-invariant readout, density surfaces, and a 2D-hypothesis / high-dimensional-verification loop documented across two domains. The public demo runs on synthetic data only.*

### [modal-analysis-portfolio](https://github.com/Yurikada/modal-analysis-portfolio)

実験モード解析のPythonツールキットです。LSCF安定化ダイアグラム、CMIF、共有ポールMIMOフィッティングを実装し、正解値付き合成データと再現可能な検証スクリプトで照合しています。

*Experimental modal-analysis toolkit validated against synthetic systems with known modal parameters.*

### [geo-change-detection](https://github.com/Yurikada/geo-change-detection)

Sentinel-2画像から山火事前後の変化を検出し、Copernicus EMSの公式被害評価と照合したケーススタディです。分光指数、Otsu閾値、モルフォロジ、評価指標の計算核を実装し、確立ライブラリとの数値一致と、外した予測の訂正過程を残しています。

*Wildfire change detection from Sentinel-2 imagery, evaluated against Copernicus EMS reference data.*

### [bayesopt-process](https://github.com/Yurikada/bayesopt-process)

ベイズ最適化を、ガウス過程、獲得関数、ノイズ、バッチ評価、校正まで段階的に検証した実験プロジェクトです。自前実装を外部実装と照合し、手法の優位性が問題設定に依存することも含めてレポート化しています。

*A staged Bayesian-optimization study covering Gaussian processes, acquisition functions, noise, batching, and calibration.*

## How I work

- 変更前に仮説と比較条件を置く
- 指標を参照定義、分母、測定限界とセットで読む
- 自前実装は手計算または確立ライブラリと照合する
- 予測を外した場合も削除せず、原因と訂正を記録する
- 実装済み、推論、未検証を分けて説明する

## Profiles

- [Kaggle: yosukeinada](https://www.kaggle.com/yosukeinada)
