achemso を使って、latex原稿をarXivに投稿する方法。

\setkeys{acs}{articletitle=true, doi=true}
の行ありでコンパイル。

pdflatex, pdflatex, bibtex, pdflatex, pdflatex
ここでbblができている。

さっきの行をコメントアウトする。
%\setkeys{acs}{articletitle=true, doi=true}

bib とbbl, 必要なFigureのpdfを、tar.gzにまとめてアップロードする。
