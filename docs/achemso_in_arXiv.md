achemso を使って、latex原稿をarXivに投稿する方法。
-----

1. 下記の行がtexにある状態でコンパイルする。(pdflatex, pdflatex, bibtex, pdflatex, pdflatex)
````
\setkeys{acs}{articletitle=true, doi=true}
````

2. これでbblファイルができているはず。

3. さっきの行をコメントアウトしておく。
````
%\setkeys{acs}{articletitle=true, doi=true}
````

4. bib とbbl, 必要なFigureのpdfを、tar.gzにまとめてアップロードする。
