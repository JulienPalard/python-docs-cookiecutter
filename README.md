# Cookiecutter to bootstrap a new Python documentation translation

## Bootstraping a Python documentation translation

You will be asked for the language of your translation, please give an
IETF language code, lowercased, with dashes. like "pt-br", "fr", "ja",
"zh-cn", and so on.

    $ git clone https://github.com/python/cpython.git
    $ (cd cpython; git checkout 3.7)
    $ pip install cookiecutter
    $ cookiecutter https://github.com/JulienPalard/python-docs-cookiecutter
    language [fr]: de
    directory_name [python-docs-de]:
    $ cd python-docs-de
    $ make merge
    $ git init
    $ git add *.po */*.po README.rst Makefile
    $ git commit -m "Initial commit"
