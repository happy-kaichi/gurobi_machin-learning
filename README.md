#  小売価格最適化：機械学習 × Gurobi による意思決定支援

本プロジェクトでは、機械学習を用いた需要予測と、Gurobi最適化ソルバーによる価格最適化の統合を通じて、小売商品の価格戦略を数理的に導出する方法を実装・検証しています。

---

##  プロジェクト構成

| ファイル名                               | タグ             | 内容説明 |
|------------------------------------------|------------------|----------|
| `retail_price_optimization.ipynb`        | `notebook`       | 機械学習モデル構築とGurobiによる価格最適化のJupyter Notebook |
| `プレゼンテーションスライド.pdf`         | `presentation`   | プロジェクトの概要・手法・結果・考察をまとめたスライド |


---

##  プロジェクトの概要

- Gurobi × 機械学習を活用した価格最適化手法を提案
- 需要予測モデル（線形回帰）を学習し、予測された売上数量と価格の積（売上）を最大化
- Gurobi の `gurobi-machinelearning` パッケージにより、MLモデルを直接最適化制約に組み込み

---

##  使用技術

- Python 3.x
- pandas / matplotlib / seaborn / scikit-learn / plotly
- Gurobi Optimizer 10.0
- gurobi-machinelearning（Gurobi社公式パッケージ）

---

## 📊 成果のハイライト

- MLモデルによる需要予測精度：R² = 0.294
- Gurobiにより現実的な価格制約を加味した最適解を導出
- 最適化前と比較して売上が **約449,000円 → 約490,000円** に改善

---

##  学べるポイント

- `gurobi-machinelearning` を使った ML × 最適化の統合手法
- 数値最適化の定式化と実装（目的関数、価格制約、在庫制約など）
- 可視化による予測精度と価格戦略の検証方法

---

## 🔗 参考文献・リンク

- 📘 [Gurobi Machine Learning GitHub](https://github.com/Gurobi/gurobi-machinelearning)
- 📊 [スライド：Using Trained ML Predictors in Gurobi (公式)](https://cdn.gurobi.com/wp-content/uploads/Using-Trained-Machi)
