<!-- ELUCENIA technical documentation · boston-bowel-preparation-scale · zh · no clinical/professional/rights approval -->

# Boston 肠道准备量表（BBPS）

[条件、来源与许可](https://elucenia.org/zh/tools/boston-bowel-preparation-scale)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 右半结肠（盲肠及升结肠）

`dir`

- `0` — 0 – 黏膜不可见（固体粪便）
- `1` — 1 – 部分黏膜可见
- `2` — 2 – 少量残留，黏膜可清楚观察
- `3` — 3 – 全部黏膜可清楚观察

### 横结肠（包括结肠曲）

`trans`

- `0` — 0 – 黏膜不可见（固体粪便）
- `1` — 1 – 部分黏膜可见
- `2` — 2 – 少量残留，黏膜可清楚观察
- `3` — 3 – 全部黏膜可清楚观察

### 左半结肠（降结肠、乙状结肠及直肠）

`esq`

- `0` — 0 – 黏膜不可见（固体粪便）
- `1` — 1 – 部分黏膜可见
- `2` — 2 – 少量残留，黏膜可清楚观察
- `3` — 3 – 全部黏膜可清楚观察

## 方法版本

BBPS/Lai 2009：3肠段，冲洗/吸引后各0–3，总分0–9

## 已记录的公式

各肠段在冲洗和吸引后评分0至3：

0：未准备，无法清除的固体粪便遮住黏膜。

1：部分黏膜可见，其余被着色、残便或不透明液体遮挡。

2：少量残留，黏膜清晰。

3：全部黏膜清晰，无残留。

总分0至9。

## 限制与适用人群

BBPS旨在对内镜医师冲洗和吸引后检查所见的清洁程度评分。原始单中心研究并不自动证实后续建议中采用的充分清洁阈值或重复检查间隔。应保留对各肠段的评估及所采用标准的版本。

## 参考文献

- [Lai EJ et al. The Boston bowel preparation scale: a valid and reliable instrument for colonoscopy-oriented research. Gastrointest Endosc, 2009.](https://doi.org/10.1016/j.gie.2008.05.057)

- [Calderwood AH, Jacobson BC. Comprehensive validation of the Boston Bowel Preparation Scale. Gastrointest Endosc, 2010.](https://doi.org/10.1016/j.gie.2010.06.068)

- [Johnson DA et al. Optimizing adequacy of bowel cleansing for colonoscopy: recommendations from the US Multi-Society Task Force on Colorectal Cancer. Gastroenterology, 2014.](https://doi.org/10.1053/j.gastro.2014.07.002)

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
