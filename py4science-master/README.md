# 「科学技術計算のためのPython入門――開発基礎、必須ライブラリ、高速化」

本レポジトリは、技術評論社から出版された以下の書籍
のWeb補足情報を提供するためのものです。

<img src="cover_image.png" align="center" width="300" >

タイトル: 科学技術計算のためのPython入門――開発基礎、必須ライブラリ、高速化  
著者: 中久喜 健司（なかくき けんじ）  
単行本（ソフトカバー）: 416ページ  
出版社: 技術評論社  
言語: 日本語  
ISBN-10: 4774183881  
ISBN-13: 978-4774183886  
発売日: 2016/9/24  
技術評論社のサポートページ: http://gihyo.jp/book/2016/978-4-7741-8388-6/  

本レポジトリでは、主に書籍中のソースコードを提供するとともに、Webサポートページに
上記の書籍をサポートする情報を提供します。

GitHubレポジトリ: https://github.com/pyjbooks/py4science  
同サポートページ: https://pyjbooks.github.io/py4science/


# ソースコードについて

## ファイルの所在

本レポジトリのmasterブランチの「src」フォルダ以下に、書籍の章ごとに分けて格納してあります。Gitを使える方は、クローンして入手してください。Gitを使えない方は、本GitHubレポジトリのトップページで、[Clone or download]というボタンを押して、zipファイルとしてダウンロードしてください。

## 「改行」と「空白」
書籍の中では、紙幅の都合上、*「改行」や「空白」をわざと減らしている*部分がありますが、本レポジトリに含まれるソースコードは、PEP 8に準拠できるように改行や空白を挿入しています。

## import文の省略
また、ソースコードの冒頭に含まれるimport文についても、紙幅の都合上、書籍の中では*省略している場合があります*。以下のimport文が先頭に付いていることを前提としていますので、ご注意ください。本レポジトリに含まれるソースコードでは、省略せずに記載しています。

    import numpy as np  # NumPyの別名はnp
    import scipy as sp  # SciPyの別名はsp
    import pandas as pd  # pandasの別名はpd
    import matplotlib as mpl  # Matplotlibの別名はmpl
    import matplotlib.pyplot as plt  # Matplotlib.pyplotの別名はplt
    import numexpr as ne  # Numexprの別名はne

## Matplotlibの設定

Matplotlibの設定がユーザの環境によって異なることで、本書の中で示したプロット結果と、多少「体裁」が異なる結果が得られる場合があります。その場合には、本書の9.2項を参考に、設定をご自分で調整してみてください。

特に、本書では以下の設定を推奨しており、本書に示した図と異なる場合には以下の設定を加えてみてください。（「mpl」は上記のとおり、「matplotlib」の別名）

    mpl.rcParams['figure.autolayout'] = True
    mpl.rcParams['font.size'] = 14
    mpl.rcParams['axes.grid'] = True

また、インタラクティブモードがoffになっている場合は、プロットした図が表れない場合があります。
その場合は、`plt.ion()`（「plt」は上記のとおり「matplotlib.pyplot」の別名）として、インタラクティブモードをonにしてください。
もしくは、プロットの最後に、`plt.show()`を追加することで、図を表示させることができます。

## その他

稀に間違いが見つかった場合などに、本レポジトリのソースコードにおいては修正が加えられている場合があります。その他にも、書籍の中のソースコードに、上記のとおりimport文が加えられている場合や、軽微な修正が行われている場合があります。

# 正誤表

本レポジトリの「error_table.txt」に、本書中の誤記等の訂正を示してあります。

# ライセンス

本レポジトリのソースコードについては、「LICENSE.md」に示したとおりです。

