Symbolic execution timeline
===========================

Diagram highlights some major tools and ideas of pure symbolic execution, dynamic symbolic execution (concolic) as well as related ideas of model checking, SAT/SMT solving, black-box fuzzing, taint data tracking, and other dynamic analysis techniques.

Preview
-------

:warning: PNG preview could be outdated. See [`symbolic-execution.svg`](diagram/symbolic-execution.svg) for the latest version.

![Preview](https://raw.github.com/enzet/dynamic-symbolic-execution/master/diagram/symbolic-execution.png)

Building PNG or PDF
-------------------

Please, install fonts for correct SVG display:
  * [Roboto](https://fonts.google.com/specimen/Roboto) (regular and italic) and
  * [Fira Code](https://github.com/tonsky/FiraCode).

Use Inkscape to build:

  * PNG: `inkscape diagram/symbolic-execution.svg --export-png diagram/symbolic-execution.png --export-dpi 150`,
  * PDF: `inkscape diagram/symbolic-execution.svg --export-pdf diagram/symbolic-execution.pdf`.

Contribution
------------

Feel free to suggest changes or add new information. If your change is minor (like typo), you can just edit source code of [`symbolic-execution.svg`](diagram/symbolic-execution.svg). If change is major, you are encouraged to either create new issue, or edit `symbolic-execution.svg` ([Inkscape](https://inkscape.org/en/) editor is strongly recommended due to source code issues).

### Before commiting ###

Please, use [SVGO](https://github.com/svg/svgo) for diagram optimization before commiting (to get more clean diff):

    svgo diagram/symbolic-execution.svg \
        --pretty \
        --enable=sortAttrs \
        --disable=removeEditorsNSData \
        --disable=cleanupIDs \
        --indent=2
