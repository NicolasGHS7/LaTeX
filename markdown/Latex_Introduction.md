
# Introduction to LaTex

De Basis layout van een LaTex file is:

``` latex
\documentclass{article}
\begin{document}
    Hello World!
\end{document}
```

Sommige Statements hebben een backslash (\\)  en dit betekent dat LaTex dit niet moet interpreteren als gewone tekst, maar wel als een instructie of commando voor de LaTex compiler.
Deze instructies hebben deze structuur: ``\commandname{option}``

- Het eerste deel staat voor de naam van de instructie en in de haakjes staat een optie voor de instructie.

We gaan nu een beetje dieper kijken naar de instructie ``\documentclass{article}``. Deze instructie noemt duidelijk "documentclass" en zet de document class (naar article) .

LaTex gebruikt klassen om de layout te bepalen van jouw document, er is bijvoorbeeld een klasse om een layout te maken van artikelen, boeken of nog veel meer die we nu niet zullen bekijken. 

Het 2de voorbeeld verschilt wat van het eerste, omdat de instructie een ``\begin`` en ``\end`` statement bevat. Eigelijk is dit zelfs geen instructie maar wel een environment. Een environment is een soort area binnen in jouw document waar een soort typesetting is. In dit voorbeeld wordt getoont hoe environments gebruikt kunnen worden:

``` latex
\begin{document}
    \begin{environment1}
        \begin{environment2}
        \end{environment2}
    \end{environment1}
\end{document}          
```

# Adding a Title page

Terwijl het mogelijk is je eigen environments te maken, is de kans groot dat degene je wilt al bestaat. LaTex heeft al redelijk veel gemaakte environments die je kan gebruiken.

``` latex
\documentclass{article}

\title{My First Document}
\date{2013-09-01}
\author{John Doe}

\begin{document}
    \maketitle
    \newpage

    Hello World!
\end{document}
```

# Latex paragraphs en sections gebruiken

Doormiddel van sections en paragraphs breng je structuur in je document. Dit is een introductie tot headings en de basic file layout van Latex.

## Sectioning elements (sections, subsections, paragraphs, ...)

Bij het schrijven van een paper is het zeer belangrijk om een logische en overzichtelijke structuur aan te brengen. Latex heeft instructies  waarbij er verschillende dingen zoals headings of sections automatisch komen. De instructies om een headings section te creëren:

``` latex
\section{}
\subsection{}
\subsubsection{}

\paragraph{}
\subparagraph{}
```

## De output van sections en subsections

De section instructies zijn genummerd en zullen getoont worden in de table of contents van jouw document. Paragraphs zijn niet genummerd en worden niet getoont in de table of contents. (zie example_sections.tex)

