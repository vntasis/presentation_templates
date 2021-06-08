---
title:
- 'My study'
author:
- My name
institute:
- My group
date:
- 23/10/2020
bibliography:
- ../../papers/bib.bib
biblio-title: References
biblio-style: nature
biblatexoptions:
- backend=biber
- citestyle=authoryear
- maxcitenames=3
- maxbibnames=15
aspectratio: 169
toc: true
theme:
- default
colortheme:
- whale
outertheme:
- infolines
innertheme:
- circles
fonttheme:
- structuresmallcapsserif
header-includes:
- |
  ```{=latex}
  % latex code that introduces slide page number
  \setbeamertemplate{footline}{%
    \raisebox{5pt}{\makebox[\paperwidth]{\hfill\makebox[20pt]{\color{gray}
      \scriptsize\insertframenumber}}}\hspace*{5pt}}
  \beamertemplatenavigationsymbolsempty
  \setbeamercolor{section in head/foot}{bg=black,fg=white}
  \setbeamercolor{itemize item}{fg=black}
  %\setbeamercovered{transparent} % For making pauses transparent instead of invisible.
  %\setbeameroption{show notes} % For creating extra slides with the notes on them.
  %\setbeamertemplate{note page}[plain] % For converting the slides that include the notes into a plain format.
  \usepackage[overridenote]{pdfpc} % For including the notes in the presentation using pdfpc (not in extra slides).
  \usepackage{multimedia}
  \titlegraphic{
    \includegraphics[height=1cm,keepaspectratio]{../../pictures/artix.png}%
    \hfill%
    \includegraphics[height=1cm,keepaspectratio]{../../pictures/arch-2.jpg}%
  }
  ```
---
# Section1

## Subsection 1.1

### Slide 1

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

### Slide 2

<!---
incremental list
-->

:::incremental

- Item 1
- Item 2
- Item 3

:::

## Subsection 1.2

### Slide 3

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

# Section 2

## Subsection 2.1

### Slide 4

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

### Slide 5
<!---
Introduce a plot from a pdf file
-->

\center
\includegraphics[page=1, width=0.9\linewidth]{plots/my_analysis.pdf}

## Subsection 2.2

### Slide 6

<!---
Introduce an image
-->

![This is the caption](images/DNA.png)

### Slide 7
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

# Section 3

## Subsection 3.1
### Slide 8

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

### Slide 9

<!---
Introduce a reference
-->

Seminal work done:

- Study 1 [^fn1]
- Study 2 [^fn2]
- Study 3 [^fn3]

[^fn1]: @Gaussian_derivation
[^fn2]: @WATSON_1953
[^fn3]: @Li_2011

## Subsection 3.2

### Slide 10

<!---
Include a video that will play during presentation.
You have to use pdfpc to present.
-->

\movie{\includegraphics[height=0.8\textheight]{images/apollo17.jpg}}{images/apollo17.avi}

\note{This is a video}

### Slide 11

\centering
**Thank you for your attention!**
