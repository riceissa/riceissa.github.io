---
layout: default
title: Proving the limit laws
comments: "yes"
disqus-id: ee9b153b71076aa4d5c8e683bb33f2adb0b78f0c
math: "yes"
last-major-revision-date:
license: "CC-BY"
tags: math
---

**Addition.** Let `\(E\subset \mathbf{R}\)` be a subset of the real
numbers, `\(f, g : E \to \mathbf{R}\)` be real functions, and
`\(L_1, L_2\in \mathbf{R}\)` be real numbers. Now suppose
`\(\lim_{x\to a} f(x) = L_1\)` and `\(\lim_{x\to a} g(x) = L_2\)`. We
would like to show that `\(\lim_{x\to a} (f(x)+g(x)) = L_1+L_2\)`.

Since `\(\lim_{x\to a} f(x) = L_1\)` and `\(\lim_{x\to a} g(x) = L_2\)`,
we know that 
`\[ \forall \epsilon >0 \exists \delta >0 \forall x (0 < |x-a|<\delta
\to |f(x)-L_1|<\epsilon ) \]`
and
`\[ \forall \epsilon >0 \exists \delta >0 \forall x (0 < |x-a|<\delta
\to |g(x)-L_2|<\epsilon).\]`
Now let `\(\epsilon > 0\)`. We need to find `\(\delta > 0\)` such that
`\[
0<|x-a|<\delta \to |(f(x)+g(x))-(L_1+L_2)|<\epsilon.
\]`
But
`\[
\begin{align}|f(x)+g(x)-(L_1+L_2)| &= |f(x)-L_1 + g(x)-L_2| \\
&\leq |f(x)-L_1| + |g(x)-L_2|.\end{align}
\]`


