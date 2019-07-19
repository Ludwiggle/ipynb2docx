# ipynb2docx

Convert Juyter Notebooks to docx preserving LaTeX formatting. 

## Requirements

* [Jupyter](https://jupyter.org/)
* [Wolfram Engine](https://www.wolfram.com/engine/)
* [mathjax-node](https://www.npmjs.com/package/mathjax-node)
* [librsvg2-bin](https://en.wikipedia.org/wiki/Librsvg)
* [pandoc](https://pandoc.org/installing.html#linux)

## Usage

`$ ipynb2docx <notebook.ipynb>`

### How it works

It converts the notebook to html with `jupyter-nbconvert`, then LaTeX math and equations are converted to png and embedded in the html as, and finally `pandoc` converts the html to docx.
