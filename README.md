# Yurikada

**現象を説明するモデルと、そのモデルをどこまで信頼できるか検証する仕組みを、対で作ります。**

*I build models of real-world phenomena together with checks that make their evidence and limits explicit.*

機械工学、振動・モード解析、設備診断の経験を基盤に、数値計算、統計、機械学習を用いた検証可能な成果物を作っています。結果だけでなく、比較条件、評価基準、外した予測、残る限界まで記録することを重視しています。

My background is in mechanical engineering, vibration analysis, and equipment diagnostics. I build reproducible numerical and machine-learning case studies, with explicit baselines, validation criteria, failed predictions, and limitations.

## Representative work

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
