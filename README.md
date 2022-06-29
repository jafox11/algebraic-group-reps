# Representations of Algebraic Groups on the Nullcone

Let $G$ be an algebraic group defined over an algebraically closed field $k$, and let g be its Lie algebra.  Let $N$ be the nullcone of g, which is the algebraic variety consisting of the nilpotent elements of g.  Let $k[N]$ be the coordinate ring of $N$, which is graded by homogeneous degree: $k[N]=\oplus_{n\geq 0}k_n[N]$.  When $k=\mathbb{C}$, $k_n[N]$ decomposes into the sum of finite-dimensional simple $G$-modules, which are the simple highest weight modules determined by the action of $G$ on g.  The _multiplicity_ of a highest weight module in $k_n[N]$ is the number of times it shows up as a summand in the decomposition of $k_n[N]$.

In his paper "Characters of the Nullcone" (Math. Ann., volume 252 no. 3 (1980), pages 179-182), Wim Hesselink derived a formula which gives the multiplicities of the simple highest weight modules in $k_n[N]$ for each n.

# My Contribution

A student researcher and I developed a Jupyter notebook which implements Hesselink's formula in SageMath.  Being able to see specifically how this formula works allowed me to adapt Hesselink's approach to a related situation (where we'll assume that $k$ is still algebraically closed but that it has positive characteristic).  

Suppose $G$ is equipped with an involution $t$.  Then g will also have be equipped with an involution, and it will decompose g into +1 and -1 eigenspaces k and p, respectively.   The subgroup $K$ of $t$-fixed points of $G$ acts on the nullcone $N$ of p and thus on its coordinate ring $k[N]$.  We can now ask about the multiplicity of the simple highest weight modules in $k_n[N]$ (where multiplicity now refers to the number of times such a module shows up as a composition factor in a composition series for $k_n[N]$, since we can no longer assume $k_n[N]$ is semisimple when char$(k)>0$).

The results of this multiplicity calculation were published in _Communications in Algebra_ in 2021.

# Files Included in This Repository

* Hesselink's 1980 paper from _Mathematische Annalen_.
* My student's and my Jupyter notebook which implments Hesselink's formula using SageMath.
* My related _Communications in Algebra_ paper from 2021.
