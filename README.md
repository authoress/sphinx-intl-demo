# Sphinx-intl demo project

This repository contains a demo project that shows the result of using *sphinx-intl* to [localize documentation created with Sphinx](http://sphinx-intl.geekwriter.ru/en/).

The **zen** directory contains the demo project, translated from English into Russian and Portuguese, ready to be built. 
Note that easter-egg.po in zen/locale/pt_br/LC_MESSAGES is intentionally left untranslated so that you can [translate it with Transifex](http://sphinx-intl.geekwriter.ru/en/translate-text-in-po-files.html#using-transifex).

Before you build the demo documentation, be sure to install Sphinx:

`pip install sphinx`

If you plan to add or change translations, you will also need Sphinx-intl:

`pip install sphinx-intl`

Of course, you can install the exact packages I have installed in my demo environment:

`pip install -r requirements.txt`

To build the project on Windows:

1. Run cmd.
2. Go to the project directory.
3. Run these commands in sequence: 
   
   `sphinx-build -b html -D language=en -d _build/doctrees/en/ . _build/html/en/`
   
   `sphinx-build -b html -D language=ru -d _build/doctrees/ru/ . _build/html/ru/`
   
   `sphinx-build -b html -D language=pt_BR -d _build/doctrees/pt_BR/ . _build/html/pt_BR/`
   
For more information, see Step by step guide [in English](http://sphinx-intl.geekwriter.ru/en/) or [in Russian](http://sphinx-intl.geekwriter.ru/).
