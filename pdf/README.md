## To build LaTeX --> .pdf

cd into the conversion_tools directory. Run the main script in nb2latex.py

```
$ conda activate book
(book)$ cd conversion_tools
(book)$ python nb2latex.py
```

open ```/pdf/pdfout3.tex``` in TexWorks. Put a ```*``` by the Preface chapter header and the appendix chapter header. Follow with a line to add the chapter back to the table of contents.

```
\chapter*{Preface}\label{preface}
	\addcontentsline{toc}{chapter}{Preface}
```

Also do this with the sections of the preface. So the first section needs to be changed to

```
 \section*{Motivation}\label{motivation}
        \addcontentsline{toc}{section}{Motivation}
```

 Typeset with XeLaTeX twice to produce .pdf

 Note: to make a section double column (really to make the section be surrounded by the ```\begin{problems}``` and  ```\end{problems}```): View the cell metadata, and inside the metadata include the JSON:

 ```
 {
  "latex": {
    "environment": "problems"
  }
}
```
