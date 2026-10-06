<!-- ELUCENIA technical documentation · volume-prostatico · ja · no clinical/professional/rights approval -->

# 前立腺体積（楕円体モデル）

[条件・出典・許諾](https://elucenia.org/ja/tools/volume-prostatico)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 縦径（頭尾方向）

`long`

cm · 範囲: 1–15

### 横径（左右方向）

`transv`

cm · 範囲: 1–15

### 前後径

`ap`

cm · 範囲: 1–15

### 総PSA（任意、密度用）

`psa`

ng/mL · 任意 · 範囲: 0.1–1000

## 方法の版

楕円体π/6×3径/Terris–Stamey 1991、PSA密度=PSA/容積

## 記載された計算式

容積 (mL) = π/6 × 縦径 × 横径 × 前後径 (cm), 約 0.52 × 3計測の積.

PSA密度 = PSA ÷ 容積.

## 限界・対象集団

楕円体の式は幾何学的な近似です。引用された研究では、経直腸超音波による推定を手術標本の重量と比較し、方法と大きさによって性能が異なることを観察しました。MRIと超音波の同等性や、PSA密度による診断を自動的に確定するものではありません。

## 参考文献

- [Terris MK, Stamey TA. Determination of prostate volume by transrectal ultrasound. J Urol, 1991.](https://doi.org/10.1016/S0022-5347(17)38508-7)

- [Lerner LB et al. Management of lower urinary tract symptoms attributed to benign prostatic hyperplasia: AUA guideline part I, initial work-up and medical management. J Urol, 2021.](https://doi.org/10.1097/JU.0000000000002183)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 記録された結果

以下の情報は、合成例に対する手法の出力を保持したものです。独立した臨床的検証を示すものではありません。

### 1

前立腺肥大（30～80 mL）

| 結果の詳細 | |
| --- | --- |
| 楕円体式（π/6 ≈ 0.52） | 4.0 × 4.5 × 3.5 cm |


### 2

前立腺肥大（30～80 mL）

| 結果の詳細 | |
| --- | --- |
| 楕円体式（π/6 ≈ 0.52） | 5.0 × 6.0 × 5.0 cm |
| PSA密度 | 0.05 ng/mL/cm³ |


### 3

著明に増大した前立腺（> 80 mL）

| 結果の詳細 | |
| --- | --- |
| 楕円体式（π/6 ≈ 0.52） | 6.0 × 7.0 × 6.0 cm |

