---
title:
- 'My study'
author:
- My name
date:
- 13/10/2020
theme:
- Copenhagen
header-includes:
- |
  ```{=latex}
  % latex code that introduces slide page number
  \setbeamertemplate{footline}{%
    \raisebox{5pt}{\makebox[\paperwidth]{\hfill\makebox[20pt]{\color{gray}
      \scriptsize\insertframenumber}}}\hspace*{5pt}}
      \beamertemplatenavigationsymbolsempty
  ```
---

# Slide 1

<!---
This is a comment.
This is a simple example of using mardown and pandoc to make a beamer presentation.
You could render this file into a pdf presentation by typing:
pandoc mrkdn_template.md -t beamer -o my_presentation.pdf
-->

\center
The objectives of the current study are...

\pause
\vfill

Write a bit more about it...

# Slide 2

<!---
incremental list
-->

:::incremental

- Item 1
- Item 2
- Item 3

:::

# Slide 3

<!---
write display mode mathematical expressions in latex
-->

$$
x^n + y^n = z^n
$$
\pause
\vfill
\centering

<!---
write inline mathematical expressions in latex
-->

$E=mc^2$


# Slide 4

<!---
Columns - Split slide vertically
-->

:::::::::::::: {.columns align=center}
::: {.column width="50%"}
\centering
**Title 1**
This is important, because...
:::
::: {.column width="50%" align=center}
\centering
**Title 2**
This is a minor issue, due to...
:::
::::::::::::::

# Slide 5
<!---
Introduce a plot from a pdf file
-->

\includegraphics[page=1, width=0.9\linewidth]{plots/my_analysis.pdf}

# Slide 6

<!---
Introduce an image
-->

![This is the caption](images/DNA.png)

# Slide 7
<!---
Introduce boxes for highlighting
-->

\begin{block}{Remark}
Sample text
\end{block}

\begin{alertblock}{Important theorem}
Sample text in red box
\end{alertblock}

\begin{examples}
Sample text in green box. The title of the block is ``Examples".
\end{examples}

# Slide 8

<!---
A simple workflow plot with pauses
-->

\centering
\framebox[1.3\width]{Step 1} \pause
$$\Downarrow$$
\framebox[1.3\width]{Step 2} \pause
$$\Downarrow$$
\framebox[1.3\width]{Step 3} \pause
$$\Downarrow$$
\framebox[1.3\width]{Step 4}

# Slide 9

\centering
**Thank you for your attention!**
