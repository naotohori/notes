achemso を使って、latex原稿をarXivに投稿する方法。
-----

1. 下記の行がtexにある状態でコンパイルする。(pdflatex, pdflatex, bibtex, pdflatex, pdflatex)
  ````
  \setkeys{acs}{articletitle=true, doi=true}
  ````
1. これでbblファイルができているはず。
1. さっきの行をコメントアウトしておく。
  ````
  %\setkeys{acs}{articletitle=true, doi=true}
  ````
1. bib とbbl, 必要なFigureのpdfを、tar.gzにまとめてアップロードする。
