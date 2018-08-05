## To build LaTeX --> .pdf

cd into the conversion_tools directory. Run the main script in nb2pdf.py

```
$ conda activate book
(book)$ cd conversion_tools
(book)$ python nb2pdf.py
```

open ```/pdf/pdfout3.tex``` in TexWorks. Put a ```*``` by the Preface chapter header and the appendix chapter header. Typeset with XeLaTeX twice to produce .pdf
