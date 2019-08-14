# 概要説明
このリポジトリは、3Sセメスターの生物情報科学実験の岩崎先生のタームで取り組んだ課題2のためのリポジトリです。複数の既存のソフトウェアを用いて、dN/dS解析をおこなっています。
必要なソフト(clustal omega)をインストールし、このリポジトリをcloneし、ipynb(deinococcus_radiodurans_r1_thermus_thermophilus_hb_ds_dn_analysis.ipynb もしくは、deinococcu_radiodurans_r1_deinococcus_gobiensis_i0_ds_dn_analysis.ipynb)を開いてコマンドを実行することで、解析を再現することができます。

# ディレクトリの意味
この解析では既存のいくつかのソフトウェアを利用しているため、その実行ファイルもこのリポジトリに含まれています。
以下が、使用したソフトウェアです。
* codeml
	* codeml/bin/codemlが実行ファイルです。
* pal2nal
	* pal2nal.v14/pal2nal.plが実行ファイルです。
* clustal omage
	* clustal omegaはローカルにインストールして用いましたが、パッケージを用いてインストールしたため、このリポジトリに実行ファイルをおいていません。再現する場合は、ローカルにclustal omegaをインストールして実行してください。

その他のディレクトリ構成について
* clustal_input
	* clustal_omegaに入力するファイル群
* clustal_output
	* clustal omegaから出力されたファイル群
* pal2nal_input
	* pal2nalに入力するファイル群
* pal2nal_output
	* pal2nalから出力されたファイル群
* codeml_input
	* codemlに入力するファイル群
* codeml_output
	* codemlから出力されたファイル群
* codeml_control
	* codeml実行に必要な設定ファイル群

* data
	* NCBIなどのデータベースから取得した、解析に用いるデータ群
	* 今回用いていないデータも格納されています。
* report
	* 提出したレポートとそれをの作成するためのLaTex用ファイル群

* deinococcus_radiodurans_r1_deinococcus_gobiensis_i0_ds_dn_analysis.ipynb
	* deinococcus radiodurans r1とdeinococcus gobiensis i0を比較してdN/dS解析するメインのファイル。これを逐一実行することで、各ソフトウェアの入出力ファイルが上記のディレクトリに作られ、最終的にdN/dS値をプロットしたグラフを表示する。

* deinococcus_radiodurans_r1_thermus_thermophilus_hb_ds_dn_analysis.ipynb
	* deinococcus radiodurans r1とthermus thermophilus hbを比較してdN/dS解析するメインのファイル。これを逐一実行することで、各ソフトウェアの入出力ファイルが上記のディレクトリに作られ、最終的にdN/dS値をプロットしたグラフを表示する。

* その他のファイル
	* これ以外のファイルは、codemlの出力としてプログラムを実行した場所と同じディレクトリに生成される出力ファイルです。codemlの出力ファイルではありますが、出力先の指定が容易ではなかったこと、今回の解析では用いなかったことから、今回は無視していただいて構いません。
	* 以下のファイルです、
		* 2ML.dN
		* 2ML.dS
		* 2ML.t
		* 2NG.dN
		* 2NG.dS
		* 2NG.t
		* rst
		* rst1
		* rub

	
# 参考文献
レポート用pdf作成に用いたTexのエラーで、参考文献のリンク先を載せられなかったため、こちらに記載しています

  [1] Daniel C.Jeffares et all.(2015)「A Beginners Guide to Estimating the Non-synonymous to Synonymous Rate Ratio of all Protein-Coding Genes in a Genome」

  [Available at]https://www.researchgate.net/publication/268231340_A_Beginners_Guide_to_Estimating_the_Non-synonymous_to_Synonymous_Rate_Ratio_of_all_Protein-Coding_Genes_in_a_Genome
  (参照日2019-08-14)

  [2] M.Adachi (2019) 「Extended Structure of Pleiotropic DNA Repair-Promoting Protein PprA from Deinococcus radiodurans」

  [Available at]https://www.qst.go.jp/site/press/20784.html
  (参照日2019-08-14)

  [3] Ziheng Yang(2017)「PAML Manual User Guide」

  [Availablet at] http://abacus.gene.ucl.ac.uk/software/pamlDOC.pdf

  (参照日2019-08-14)

