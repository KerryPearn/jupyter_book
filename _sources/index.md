# Getting started with Jupyter Books

## Install requirements
`pip install jupyter-book`
`pip install ghp-import`

## Method overview

1. Setup repo on GitHub
1. Clone repo to local computer
1. Add some content
1. Add a new file in the directory: rename it `_toc.yml`. Give it some content.


Add 1 page at a time and add contents to tabel fo contents

### Can install this spellchecker for jupyter lab
conda install -c conda-forge jupyterlab-spellchecker

# Build book
`jupyter-book build ./`
`ghp-import -n -p -f _build/html`

In the directory GitHub/jupyter_book/_build/html/index.html  If click on this then opens the book, but not live yet.

Go to GitHub and in settings, select pages, and there will see the link to the jupyter book on line (hosted by github)




(base) kerry@pop-os:~$ gedit .bashrc
add in two new lines:

alias j="jupyter-lab"

alias book="jupyter-book build ./ && ghp-import -n -p -f _build/html"