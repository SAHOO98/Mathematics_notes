# How to use these markdowns
There are mainly two ways to viewing. 
1. Use [Obsidian](https://obsidian.md/) or similar sort of software. I'm using Obsidian to edit and view. Obsidian can also be used to get a pdf export.
2. Use [Pandoc](https://pandoc.org/) to convert a mds to html as a final distributing document which can be viewed on any webrowser. *Theoretically pandoc can be used to render pdfs but there will be some technical issues, since the math typesetting is done in [Mathjax](https://www.mathjax.org/) not pure [latex](https://www.latex-project.org/get/)* 

## Commands in pandoc
There is a [latex_header.md](./latex_header.md) which contains some tex macros for ease of wriring. This should be appended to all md files to render it properly. Following is a the way to do.

> pandoc -s -o \[output_file.html\] latex_header.md \[any of the markdown\]  --mathjax --metadata title="your choice"


Example:-
> pandoc -s -o analysis.html latex_header.md Analysis.md  --mathjax --metadata title="Anallysis"

This will create [analysis.html](./analysis.html) .



