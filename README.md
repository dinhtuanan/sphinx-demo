# sphinx-demo

# Installation
1. python -m venv venv
2. .\venv\Scripts\activate
3. pip install -r requirements.txt
4. sphinx-quickstart docs

> Separate source and build directories (y/n) [n]: Write “y” (without quotes) and press Enter.

> Project name: Write “Lumache” (without quotes) and press Enter.

> Author name(s): Write “Graziella” (without quotes) and press Enter.

> Project release []: Write “0.1” (without quotes) and press Enter.

> Project language [en]: Leave it empty (the default, English) and press Enter.

5. Run docs: sphinx-build -M html docs/source/ docs/build/
6. Open docs/build/html/index.html in browser

# Tutorial
1. To build docs:
    - sphinx-build -M html docs/source/ docs/build/
    or
    - cd /docs
    - make html
2. change theme in conf.py (html_theme). You can add third-party theme like readthedocs but must pip install sphinx_rtd_theme
3. Create new page in /docs/source/your_new_page.rst
4. Add your page to toctree::