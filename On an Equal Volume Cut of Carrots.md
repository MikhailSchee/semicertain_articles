# On the Equal Volume Cut of Conical Carrots

<script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.5/MathJax.js?config=TeX-MML-AM_CHTML" async></script>

Mikhail Schee

## Abstract

<div markdown=1 style="text-align: justify">
In order to split an idealized conical carrot into two pieces of equal volume, a cut should be made parallel to the base and approximately one fifth of the carrots total length measured up from the bottom. This simple rule of thumb warrants real world testing.
</div>

## Motivation

<div markdown=1 style="text-align: justify">
It is of interest to cut a carrot into two pieces of equal volume. A trivial solution is to make a cut lengthwise from the tip to the base. However, this is often inconvenient because the carrot may be curved, longer than the knife's blade, or both. Therefore, the cut shall be made across the shorter dimension. 
<br><br>
Fully grown carrots generally taper significantly from one end to the other [citation needed]. In order to get a rough estimate for the position of the equal volume cut, an idealized model shall be adopted where the carrot is represented as a cone. It should be noted that by invoking Cavalieri's Principle, the following derivation can reasonably be applied to mildly curved carrots [1]. % https://en.wikipedia.org/wiki/Cavalieri%27s_principle
</div>

## Derivation

<div markdown=1 style="text-align: justify">
Consider an idealized conical carrot of length $L$ and a circular base of radius $r$ (Figure \ref{fig:carrot}). The volume of this carrot is
	$$\begin{align}\label{V}
		V = \frac{1}{3}\pi r^2 L.
	\end{align}$$

%	\begin{figure}[h!]
%		\centering
%		\includegraphics[width=0.5\linewidth]{CCFig1.JPG}
%		\caption{\textit{An idealized conical carrot. Original figure.}}
%		\label{fig:carrot}
%	\end{figure}

A fraction $k$ will define where the cut should be made. The length of the base piece will be $kL$ and the length of the tip piece will be $L-kL$. The circle formed by the cut is defined to have a radius $r_k$ (Figure \ref{fig:cutcarrot}). 

%	\begin{figure}[h!]
%		\centering
%		\includegraphics[width=0.5\linewidth]{CCFig2.JPG}
%		\caption{\textit{The conical carrot with a cut a distance $kL$ from the base. Original figure.}}
%		\label{fig:cutcarrot}
%	\end{figure}

Since the cut is defined so the volumes of the base piece and the tip piece are equal, it is only necessary to find one of those volumes for this derivation. The tip piece is a cone and its volume is given by 
	$$\begin{align}\label{tipVol}
		V_1 = \frac{1}{3}\pi r_k^2 (L-kL).
	\end{align}$$

In order to find $r_k$ in terms of $r$ and $k$, consider the two right triangles shown in Figure \ref{fig:triangles}. The triangles were formed by drawing a line from the center of the base to the tip of the carrot. Because they share the angle $\theta$, the trigonometric relation
	$$\begin{align}\label{bigT}
		\text{tan}(\theta) = \frac{r}{L}
	\end{align}$$

can be defined for the big triangle and the similar relation
	$$\begin{align}\label{lilT}
		\text{tan}(\theta) = \frac{r_k}{L-kL}
	\end{align}$$

can be defined for the smaller triangle. 

%	\begin{figure}[h!]
%		\centering
%		\includegraphics[width=0.5\linewidth]{CCFig3.JPG}
%		\caption{\textit{Two right triangles formed by the full carrot and the tip piece. Original figure.}}
%		\label{fig:triangles}
%	\end{figure}

Setting equations \eqref{bigT} and \eqref{lilT} equal to each other allows for $r_k$ to be found in terms of $r$ and $k$:
	$$\begin{align}
		\frac{r_k}{L-kL} &= \frac{r}{L}
	\end{align}$$
	$$\begin{align}
		r_k &= \frac{r}{L}(L-kL)\nonumber \\
		r_k &= r(1-k).
	\end{align}$$

This may be substituted into equation (\ref{tipVol}) to redefine the tip piece's volume:
	$$\begin{align}
		V_1 &= \frac{1}{3}\pi [r(1-k)]^2 (L-kL)\nonumber\\
		V_1 &= \frac{1}{3}\pi r^2 (1-k)^2 L(1-k)\nonumber\\
		V_1 &= \frac{1}{3}\pi r^2 (1-k)^3 L \label{tipVol2}
	\end{align}$$

Because the tip and base pieces are of equal volume, the total volume $V$ will be equal to twice the tip piece's volume.
	$$\begin{align}
		V = 2\cdot V_1
	\end{align}$$

Substituting equations $(\ref{V})$ and (\ref{tipVol2}) into the above expression gives
	$$\begin{align}
		 \frac{1}{3}\pi r^2 L &= 2\cdot \frac{1}{3}\pi r^2(1-k)^3 L.
	\end{align}$$

Canceling common factors from both sides leaves a relatively simple expression for $k$.
	$$\begin{align}
		1 &= 2(1-k)^3\nonumber\\
		\left(\frac{1}{2}\right)^{1/3} &= 1-k\nonumber\\
		k &= 1 - \left(\frac{1}{2}\right)^{1/3}
	\end{align}$$

Evaluated numerically, $k = 0.2063$ which is reasonably close to a fifth.
	$$\begin{equation}
		\boxed{k \approx \frac{1}{5}}
	\end{equation}$$
	
The equal volume cut of a conical carrot is approximately one fifth of the carrot's total length from the base. This simple rule warrants testing, most likely using the water displacement method to measure the volume of real, irregularly shaped carrots.
</div>