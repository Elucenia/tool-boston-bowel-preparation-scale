<!-- ELUCENIA technical documentation · boston-bowel-preparation-scale · ja · no clinical/professional/rights approval -->

# Boston腸管洗浄度スケール（BBPS）

[条件・出典・許諾](https://elucenia.org/ja/tools/boston-bowel-preparation-scale)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 右側結腸（盲腸・上行結腸）

`dir`

- `0` — 0 – 粘膜が見えない（固形便）
- `1` — 1 – 粘膜の一部が見える
- `2` — 2 – 残渣は少量、粘膜をよく観察できる
- `3` — 3 – 粘膜全体をよく観察できる

### 横行結腸（結腸曲を含む）

`trans`

- `0` — 0 – 粘膜が見えない（固形便）
- `1` — 1 – 粘膜の一部が見える
- `2` — 2 – 残渣は少量、粘膜をよく観察できる
- `3` — 3 – 粘膜全体をよく観察できる

### 左側結腸（下行結腸・S状結腸・直腸）

`esq`

- `0` — 0 – 粘膜が見えない（固形便）
- `1` — 1 – 粘膜の一部が見える
- `2` — 2 – 残渣は少量、粘膜をよく観察できる
- `3` — 3 – 粘膜全体をよく観察できる

## 方法の版

BBPS/Lai 2009：3部位、洗浄/吸引後0–3、合計0–9

## 記載された計算式

各部位は洗浄・吸引後に0～3：

0：未処置、除去できない固形便で粘膜が見えない。

1：一部の粘膜は見えるが、他は着色、残便、混濁液で隠れる。

2：少量の残留、粘膜はよく見える。

3：残留なく全粘膜がよく見える。

合計0～9。

## 限界・対象集団

BBPSは、内視鏡医が洗浄・吸引を行った後の観察で確認した清浄度を採点するために開発されました。単施設の原研究は、後の勧告で採用された適切性の閾値や再検査間隔を自動的に裏付けるものではありません。各区間の評価と、これらの基準の版を維持する必要があります。

## 参考文献

- [Lai EJ et al. The Boston bowel preparation scale: a valid and reliable instrument for colonoscopy-oriented research. Gastrointest Endosc, 2009.](https://doi.org/10.1016/j.gie.2008.05.057)

- [Calderwood AH, Jacobson BC. Comprehensive validation of the Boston Bowel Preparation Scale. Gastrointest Endosc, 2010.](https://doi.org/10.1016/j.gie.2010.06.068)

- [Johnson DA et al. Optimizing adequacy of bowel cleansing for colonoscopy: recommendations from the US Multi-Society Task Force on Colorectal Cancer. Gastroenterology, 2014.](https://doi.org/10.1053/j.gastro.2014.07.002)

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

前処置良好（合計 ≥ 6 かつ全セグメント ≥ 2）

| 結果の詳細 | |
| --- | --- |
| 右側結腸 | 3 |
| 横行結腸 | 3 |
| 左側結腸 | 3 |


### 2

前処置良好（合計 ≥ 6 かつ全セグメント ≥ 2）

| 結果の詳細 | |
| --- | --- |
| 右側結腸 | 2 |
| 横行結腸 | 2 |
| 左側結腸 | 2 |


### 3

前処置不十分：短期間で大腸内視鏡検査を再実施する

| 結果の詳細 | |
| --- | --- |
| 右側結腸 | 1 |
| 横行結腸 | 3 |
| 左側結腸 | 3 |

合計 ≥ 6 だが、スコア < 2 の区域があるため、前処置は適切とみなされない。


### 4

前処置不十分：短期間で大腸内視鏡検査を再実施する

| 結果の詳細 | |
| --- | --- |
| 右側結腸 | 1 |
| 横行結腸 | 1 |
| 左側結腸 | 1 |

