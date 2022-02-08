# Annotated example of how to make annotated equations in LaTeX using TikZ.

![output of annotated equation](example_annotation.png)

Inspired by Sibin Mohan's https://github.com/synercys/annotated_latex_equations/, but with significantly simplified TikZ code, and with lots of comments to explain what is going on.

Two versions, one for Beamer slides, one for within an article. For more complex examples, see https://github.com/synercys/annotated_latex_equations/.

## Giving all highlight boxes the same height

Simply add a `\mathstrut` within the colorbox:
```diff
-\newcommand{\highlight}[2]{\colorbox{#1!17}{$#2$}}
+\newcommand{\highlight}[2]{\colorbox{#1!17}{$\mathstrut #2$}}
```

![output of annotated equation with equal-height highlights](example_annotation_equal_height.png)

## Much more information...

...in the answers to [this TeX StackExchange question}(https://tex.stackexchange.com/q/254844/171664).
