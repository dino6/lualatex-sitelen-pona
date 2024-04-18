## Notice
This package is based on [Jack Humbert's sitelen pona pona](https://github.com/jackhumbert/sitelen-pona-pona) font (a _cleaned_ version of sitelen pona), which does the heavy lifting.

However, the font in the latest release of that repository is slightly outdated (doesn't have tonsi or kijetesantakalu). This package was made using the one in Jack's repository's head branch, which is included in this repository for convenience.

Also, this is the first LaTeX package I have ever made.

# Description
This LaTeX package adds the commands `\sitelenfont` and `\toki{*}`.

`\sitelenfont` sets the font of the current environment to `sitelen-pona-pona.otf`, which allows writing text in the style of sitelen pona. 

`\toki{*}` is equivalent to `{\sitelenfont *}`, though in math mode it is equivalent to `\text{\toki{*}}`.

For every toki pona word (available in Humbert's sitelen pona pona), this package also adds the commands `\toki*` as a shorthand for `\toki{*}` (ex. `\tokitonsi`, which is equivalent to `\toki{tonsi}`). Bare in mind that any text can be passed to `\toki`, like `\toki{jan tino li nasa}`.

This package was made for and tested with LuaLaTeX. I am not sure if the way other engines are compatible with this package.

# Usage
* Install Jack Humbert's `sitelen-pona-pona.otf` font on your machine or include the file in your LaTeX project's directory.
* Install `sitelen-pona.sty` or include it in your LaTeX project's directory.
* Import the package with `\usepackage{sitelen-pona}`.

# Example

```
\documentclass{article}

\usepackage{amssymb}
\usepackage{sitelen-pona}

\begin{document}
	Let $\tokipilin \colon \mathbb R \to \mathbb R$ be the function given by
	\[ \tokipilin(\tokimun) = \frac{2}{\sqrt \pi} \int_0^{\tokimun} e^{-\tokikon^2} d \tokikon \]

	This function is known as the \toki{elo} function.	
\end{document}
```

![compiled latex file showing the definition of the error function](https://github.com/dino6/lualatex-sitelen-pona/blob/main/example/example.png)
