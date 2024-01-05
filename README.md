## Notice
This package is based on Jack Humbert's [sitelen pona pona](https://github.com/jackhumbert/sitelen-pona-pona) font (a _cleaned_ version of sitelen pona).

However, the font in the latest release of that repository is slightly outdated. This package was made using the one in Jack's repository's head branch, which is included in this repository for convenience

Also, this is the first LaTeX package I have ever made.

# Description
This LaTeX package adds the commands `\sitelenpona` and `\sitelen{*}`.

`\sitelenpona` sets the font of the current environment to `sitelen-pona-pona.otf`, which allows writing text in the style of sitelen pona.

`\sitelen{*}` writes the sitelen symbol provided as an argument, which works in both text and math mode (though in math mode it is equivalent to `\text{\sitelen{*}}`). The argument has to be lower case and an exact match to the symbol's name.

# Usage
* Install Jack Humbert's `sitelen-pona-pona.otf` font on your machine or include the file in your LaTeX project's directory.
* Include `sitelen-pona.sty` in your LaTeX project's directory.
* Import the package with `\usepackage{sitelen-pona}`.
