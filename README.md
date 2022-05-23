# latexcommands

Repository of latex commands


soumya
LaTeX Commands

Editors - TeXstudio BEST (Ubuntu and Mac OS X), Kile (Ubuntu), TexShop (Mac OS X), TexMaker (Windows) (link), TexWorks (Windows) (link)

TeX Installation on Windows (miktex)

Tex on R (tinytex  install.packages('tinytex') )

Overleaf online

1) 

$T_{0} = 2.3 \times 10^{5}$/mL.

50\% inhibition

\textit{refineparameters}

we use a {\bf viral decay study} which

frozen at -80$^\circ$C until tested

model by $\pm$ 50\% on the log scale

\begin{equation}

\frac{dV}{dt} = - (\gamma + \overline{\beta} \overline{T_{0}}) V

\end{equation}

\begin{equation}

\label{ab_eqn}

A(t) = \left\{ \begin{array}{rcl}

    0 & \mbox{,}  & t < t_{i} \\

    \eta (t - t_{i}) & \mbox{,} & t \geq t_{i}

    \end{array}\right.

\end{equation}

2) No indent in a paragraph

\noindent    TEXT HERE

3) double spacing

include the line \usepackage{setspace} after your \documentclass line. Before your \begin{document} command,

\doublespacing

4) Square brackets

\left[             \right]

5) Tilde

\sim

6) Round brackets

\left(    \right)

7) Sum with limits

\sum_{i=1}^{n} m_{i}

8) Quotation marks in LaTeX

`` Here is a sentence in quotes ''

other tips and pitfalls in LaTeX (Top 4 LaTeX mistakes)

9) Iterated product

\prod_{w \in children[u]}

10) Iterated sum

\sum_{j=1}^{m_{ik}}

11) Giving space between two symbols in math mode

$ log_{10} \, x $

12) Multiplication sign

\times

13) reference figure or equation

\ref{fig_label}

14) Integral

P =  \int_0^{t_{d}} x(t) \mathrm{d} t

15) Lists without bullets and numbers

\begin{description}

\item[] first item

\end{description}

16) Citing url in bibtex

@misc{mytools_url,

title={{Tools for Analysis and Modeling using Differential Equations and Hierarchical Bayesian Models Applied to Within-Host Viral Dynamics Models (Open source software)}},

author={Banerjee, S.},

howpublished = "\url{https://sites.google.com/site/neelsoumya/software}",

year={2013}

}

17) Ugly hack to crop eps file (without using Adobe Illustrator)

original eps file converted to jpg at http://image.online-convert.com/convert-to-jpg

then jpg file cropped to remove whitespace at http://www.picresize.com/

18) Ugly hack 2 to crop eps file (without using Adobe Illustrator)

generate eps file, include in latex using includegraphics, compile latex file.

This generates a pdf file from eps.

Crop this PDF file using free software PDF scissors http://www.pdfscissors.com/

Then include that modified pdf in latex using includegraphics

19) height and width of images in latex

\includegraphics[width=5.9in,height=3in]{bayes_figures/R0pnpcorvids_v2.eps}

20) Multiple side by side (floating) images in latex (courtesy of Joshua Hecker)

Put \usepackage{subfig} in preamble

\begin{figure}

\centering

\subfloat[]{

%\label{fig:collection_rate_real}

%\includegraphics[width=2.9in]{poc_figures/ode_simulatedata_v3_upper1.eps}

\includegraphics[width=2.8in,height=2in]{poc_figures/ode_simulatedata_v3_upper1-eps-converted-to_scissored.pdf}

}

\subfloat[]{

%\label{fig:collection_rate_sim}

%\includegraphics[width=2.9in]{poc_figures/ode_simulatedata_v3_upper2.eps}

\includegraphics[width=2.8in,height=2in]{poc_figures/ode_simulatedata_v3_upper2-eps-converted-to_scissored.pdf}

} \\

\subfloat[]{

%\includegraphics[width=5.8in,height=4in]{poc_figures/ode_simulatedata_v3_lower.eps}

\includegraphics[width=5.8in,height=2in]{poc_figures/ode_simulatedata_v3_lower-eps-converted-to_scissored.pdf}

%\label{fig:collection_rate_unbounded}

}

\caption{Figure of ODE plot}

\label{ode_plot}

\end{figure}

21) Approximate (equation) symbol

\approx

22) Latex package and template for Nature papers

23) Capitalize first letter of word in bibtex (protect capitalization with {})

For example, the letter I is wrapped in {}

title={Scaling in the {I}mmune system },

24) Figures resized/smaller (scale)

\begin{figure}[!ht]

\begin{center}

\includegraphics[width=\textwidth,scale=0.5]{Figures/figname}

\end{center}

\caption{

Supplementary Figure: Title.

}

\label{fig_appendix}

\end{figure}

25) Asterisk for affiliation

\author{ Soumya Banerjee$^{1,2,3,4}$ $^{\ast}$ }

\begin{affiliations}

\item University of Valhalla

\\

 $\ast$ Corresponding author 

\end{affiliations}

26) Capitalize Greek symbols

% upper case lambda

\Lambda

% small case lambda is

\lambda

27) Part text and part math in equations

\mathrm{d} t

28) Infinity

\infty

29) Curly braces and square brackets within math equations

\{

If want bigger then

\big\{

courtesy link

\[

\big\[

30) Square root

\sqrt

31) Matrix in LaTeX (link)

32) Displaying code in LaTeX (link)

Use Listings package

\begin{lstlisting}

code ...

\end{lstlisting}

33) Text in math mode

$r \leftarrow \text{minimum} (1,  p ) $

34) Space in math mode

$ \;  \Lambda =  X $

35) Math symbols in latex (link)

36) Matrix in LaTeX (courtesy link here)

$$

\Sigma =

 \begin{pmatrix}

  a_{1,1} & a_{1,2} & \cdots & a_{1,n} \\

  a_{2,1} & a_{2,2} & \cdots & a_{2,n} \\

  \vdots  & \vdots  & \ddots & \vdots  \\

  a_{m,1} & a_{m,2} & \cdots & a_{m,n}

 \end{pmatrix}

 $$

37) Proportional to

\propto

$ P(\alpha) \propto $

38) Prime symbol in math (like mu prime)

\mu'

a'

39) Line break in Latex

\\

40) Vector notation in latex (bold vectors, adapted from link)

\renewcommand{\vec}[1]{\mathbf{#1}}

\vec{y_{t}}

41) Subfigure in LaTeX

\begin{figure}[!htb]

\begin{center}

   \subfigure[$M=10000$]{ \includegraphics[width=0.45\textwidth]{figures/figure1a.eps}

\label{fraction_escape_figure}} \quad

   \subfigure[$M=100000$]{\includegraphics[width=0.45\textwidth]{figures/figure1b.eps} 

\label{figure_analysis_degeneracy_SYNTHETIC}}

\end{center}

\caption{Distribution of self. 

}

\end{figure}

42) Change bibliography style to Vancouver (link)

\bibliographystyle{vancouver}

43) Cover letter template (link)

44) CV template latex (link)

45) Latex templates (link) (courtesy by Mayank Drolia)

46) Table of contents (link)

47) Special characters in LaTeX (link)

48) Colors for comments

\definecolor{additions}{rgb}{0,0.5,0}

{  \color{additions}  

THIS IS REVISED TEXT.  

}

49) Renumber latex figures in Supplementary Section (link)

50) plusminus symbol

\pm


51) References without a bib file using bibitem (link)


\begin{thebibliography}{2}

\bibitem{Friedman2010} Friedman J, Hastie T, Tibshirani R (2010) Regularization paths for generalized linear models via coordinate descent. J Stat Softw 33: 1–22.

\end{thebibliography}	


52) Limit tends to infinity

\lim_{ x \to  -\infty}  (12^{x} + 1^{x} - 10^{x} - 9^{x} ) = 1


53) Bengali in Latex (link)

	
Page updated
Google Sites
Report abuse
