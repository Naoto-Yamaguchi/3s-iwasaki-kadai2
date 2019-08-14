#環境構築

OrthFinderを使ってみようと思い、[こちら](https://qiita.com/NariseT/items/e2c90d0235316f8878d8)に従って、環境構築
~/tools/を作成して、それ以下に
まず、[Blast+を入れた](https://bi.biopapyrus.jp/seq/blast/)
URLは[ここ](ftp://ftp.ncbi.nih.gov/blast/executables/blast+/LATEST)から

パスを通した
`export PATH="$HOME/tools/ncbi-blast-2.3.0+/bin:$PATH"`

MCLクラスタリングに必要らしく


#解析の流れ
* データを取得する
* CDSとproteinに整理する
* オーソログを見つける(OrthFind?)
	それかRBB method?

[ここ](https://omabrowser.org/api/docs)を参考
sequenceから、omaidをとり、それをentry_idとしてorthologをrel_type1:1で取得
これを1つの種のある遺伝子についてみる
					それが


[ここ](https://www.biostars.org/p/216985/)
でOMAを見つけた
普通はRBHBだが、OMAも悪くないという議論があるみたい
https://www.nature.com/articles/nmeth.3830
																																																																																																																																																																								


* 整形する
* dS/dNを計算(yn00? codeml?)
* 結果をプロット

