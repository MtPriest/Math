Пространство $c$ --- пространство всех сходящихся
    последовательностей с нормой
    $\lVert x \rVert=\sup_{n\in\mathbb{N}}\lvert x_n \rvert$. Ясно, что
    $c\subset \ell_\infty$, а так как нормы на $c$ и $\ell_\infty$
    задаются одинаково, то $c$ --- это подпространство в $\ell_\infty$.

 Аксиомы нормы выполнены, так как они выполнены для пространства
    $\ell_\infty$. Пространство $c$ банахово, так как замкнуто в
    $\ell_\infty$ (см. ). Докажем это: пусть $\{x^n\}_{n=1}^\infty$ ---
    последовательность элементов пространства $c$, сходящаяся к
    некоторому $y=\{y_k\}_{k=1}^\infty\in \ell_\infty$. Надо показать,
    что $y\in c$. Для этого достаточно доказать, что последовательность
    $\{y_k\}_{k=1}^\infty$ фундаментальна. Пусть $\varepsilon>0$. Так
    как $x^n\to y$, то найдётся такой номер $n_0$, что
    $\lVert x^n-y \rVert=\sup_{m\in\mathbb{N}}\lvert x_m^n-y_m \rvert<\varepsilon/3$
    для любого $n\geqslant n_0$. Так как последовательность
    $x^{n_0}=\{x^{n_0}_p\}_{p=1}^\infty$ фундаментальна, то найдётся
    такой номер $n_1$, что
    $\lvert x^{n_0}_p - x^{n_0}_q \rvert<\varepsilon/3$ если
    $p,q\geqslant n_1$. Пусть теперь $k,l\geqslant n_1$. Тогда
    $$\begin{gathered}
        \lvert y_k-y_l \rvert=\lvert y_k-x^{n_0}_k + x^{n_0}_k - x^{n_0}_l + x^{n_0}_l - y_l \rvert\leqslant \\
        \leqslant\lvert y_k-x^{n_0}_k \rvert + \lvert x^{n_0}_k - x^{n_0}_l \rvert + \lvert x^{n_0}_l - y_l \rvert<\varepsilon/3+\varepsilon/3+\varepsilon/3 = \varepsilon.\end{gathered}$$