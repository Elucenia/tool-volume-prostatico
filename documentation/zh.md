<!-- ELUCENIA technical documentation · volume-prostatico · zh · no clinical/professional/rights approval -->

# 前列腺体积（椭球模型）

[条件、来源与许可](https://elucenia.org/zh/tools/volume-prostatico)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 纵径（头尾径）

`long`

cm · 范围: 1–15

### 横径（左右径）

`transv`

cm · 范围: 1–15

### 前后径

`ap`

cm · 范围: 1–15

### 总 PSA（可选，用于密度）

`psa`

ng/mL · 选填 · 范围: 0.1–1000

## 方法版本

椭球π/6×3径/Terris–Stamey 1991；PSA密度=PSA/体积

## 已记录的公式

体积 (mL) = π/6 × 纵径 × 横径 × 前后径 (cm), 约 0.52 × 三维测量乘积.

PSA密度 = PSA ÷ 体积.

## 限制与适用人群

椭球公式是一种几何近似。所引用研究将经直肠超声估计与手术标本重量比较，并观察到不同方法和大小间表现不同。这不能自动确认磁共振与超声的等效性，也不能由PSA密度诊断。

## 参考文献

- [Terris MK, Stamey TA. Determination of prostate volume by transrectal ultrasound. J Urol, 1991.](https://doi.org/10.1016/S0022-5347(17)38508-7)

- [Lerner LB et al. Management of lower urinary tract symptoms attributed to benign prostatic hyperplasia: AUA guideline part I, initial work-up and medical management. J Urol, 2021.](https://doi.org/10.1097/JU.0000000000002183)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026
