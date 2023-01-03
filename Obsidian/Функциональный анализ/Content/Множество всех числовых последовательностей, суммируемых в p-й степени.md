Пусть $p\geqslant 1$ и $\ell_p$ --- множество всех числовых
    последовательностей, суммируемых в $p$-й степени, то есть
    $$\textstyle
    \ell_p=\left\lbrace x=(x_1,x_2,\ldots) \mid \sum_{n=1}^\infty \lvert x_n \rvert^p < +\infty \right\rbrace.$$

Норма в $\ell_p$ определяется так:
    $\lVert x \rVert=\bigl(\sum_{n=1}^\infty \lvert x_n \rvert^p\bigr)^{1/p}$.
    Выполнение первой и второй аксиом нормы очевидны, а третья аксиома
    --- это неравенство Минковского для рядов.

Докажем полноту пространств $\ell_p$. Пусть $\{x^n\}_{n=1}^\infty$
    --- фундаментальная последовательность в $\ell_p$. Это означает, что
    для любого $\varepsilon>0$ найдется такое число $n_0$, что
    $\lVert x^n-x^m \rVert<\varepsilon$ для любых $n,m \geqslant n_0$.
    Тогда
    $$\sum_{k=1}^\infty \lvert x_k^n-x_k^m \rvert^p < \varepsilon^p, \tag{$\ast$}$$
    откуда $\lvert x_k^n-x_k^m \rvert<\varepsilon$ при
    $n,m\geqslant n_0$ для каждого $k$. Последнее неравенство означает,
    что для каждого $k$ последовательность $\{x_k^n\}_{n=1}^\infty$
    фундаментальная в $\mathbb{R}$ (или в $\mathbb{C}$). Пусть
    $x_k=\lim_{n\to\infty} x_k^n$ и $x=\{x_k\}_{k=1}^\infty$. Осталось
    доказать, что $x\in \ell_p$ и что $x^n\to x$.

Сначала докажем, что последовательность $x^n$ сходится к $x$. Из
    неравенства $(\ast)$ следует, что
    $\sum_{k=1}^j \lvert x_k^n-x_k^m \rvert^p < \varepsilon^p$ для
    каждого натурального $j$. Зафиксируем в последнем неравенстве $n$ и
    перейдем к пределу при $m\to\infty$. Получим неравенство
    $\sum_{k=1}^j \lvert x_k^n-x_k \rvert^p \leqslant \varepsilon^p,$
    верное для всех $j$. Но тогда и
    $$\sum_{k=1}^\infty \lvert x_k^n-x_k \rvert^p \leqslant \varepsilon^p. \tag{$\ast\ast$}$$
    Итак, $\lVert x^n-x \rVert\leqslant\varepsilon$ при
    $n\geqslant n_0$. Это означает, что $x^n\to x$.

Осталось доказать, что $x\in \ell_p$, то есть, что ряд
    $\sum_{k=1}^\infty\lvert x_k \rvert^p$ сходится:
    $$\sum_{k=1}^\infty\lvert x_k \rvert^p = \sum_{k=1}^\infty\lvert x_k-x_k^{n_0}+x_k^{n_0} \rvert^p\leqslant
    \sum_{k=1}^\infty\lvert x_k-x_k^{n_0} \rvert^p + \sum_{k=1}^\infty\lvert x_k^{n_0} \rvert^p < +\infty,$$
    так как первое слагаемое в силу $(\ast\ast)$ не превосходит числа
    $\varepsilon^p$, а второе не превосходит некоторой константы, так
    как $x^{n_0}\in \ell_p$.

Среди пространств $\ell_p$ наиболее интересными являются
    пространства $\ell_1$ и $\ell_2$:

1.  $\ell_1$ --- пространство абсолютно суммируемых
        последовательностей с нормой
        $\lVert x \rVert=\sum_{n=1}^\infty \lvert x_n \rvert$;

2.  $\ell_2$ --- пространство квадратично суммируемых
        последовательностей с нормой
        $\lVert x \rVert=\sqrt{\vphantom{\bigl(}\sum_{n=1}^\infty \lvert x_n \rvert^2}$.