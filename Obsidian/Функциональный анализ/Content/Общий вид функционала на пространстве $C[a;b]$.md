Общий вид функционала на пространстве $C[a;b]$ {#FOV}
----------------------------------------------

### Функции ограниченной вариации

Пусть $[a;b]\subset\mathbb{R}$. Конечное множество
$T = \{t_k\}_{k=0}^n\subset [a;b]$ называется *разбиением* отрезка
$[a;b]$, если $a=t_0<t_1<\ldots < t_n=b$.

Пусть $T$ --- разбиение $[a;b]$ и $x\colon [a;b]\to\mathbb{R}$ ---
произвольная функция. Число
$\nu(T) = \sum_{k=0}^{n-1}\lvert x(t_{k+1})-x(t_k) \rvert$ называется
*вариационной суммой* функции $x$.

Величина
$$\mathop{\mathrm{\mbox{\Large{V}}}}_a^b(x) = \sup\left\lbrace \nu(T) : T \text{ --- разбиение $[a;b]$} \right\rbrace,$$
называется *полной вариацией* функции $x$ на отрезке $[a;b]$. Если
$\mathop{\mathrm{\mbox{\Large{V}}}}_a^b(x)<+\infty$ то функция $x$
называется *функцией ограниченной вариации* (*Ф.О.В.*) на отрезке
$[a;b]$.

Свойства:

-   если функция $x$ монотонна на $[a;b]$, то
    $\mathop{\mathrm{\mbox{\Large{V}}}}_a^b(x)=\lvert x(b)-x(a) \rvert$;

-   $\mathop{\mathrm{\mbox{\Large{V}}}}_a^b(x)=0$ тогда и только тогда,
    когда $x=\text{const}$;

-   $\mathop{\mathrm{\mbox{\Large{V}}}}_a^b(\alpha x) = \lvert \alpha \rvert\mathop{\mathrm{\mbox{\Large{V}}}}_a^b(x)$;

-   $\mathop{\mathrm{\mbox{\Large{V}}}}_a^b(x+y)\leqslant \mathop{\mathrm{\mbox{\Large{V}}}}_a^b(x) + \mathop{\mathrm{\mbox{\Large{V}}}}_a^b(y)$;

    Доказательство. $$\begin{gathered}
    \sum_{k=0}^{n-1}\lvert (x+y)(t_{k+1})-(x+y)(t_k) \rvert\leqslant\\
    \leqslant\sum_{k=0}^{n-1}\lvert x(t_{k+1})-x(t_k) \rvert+\sum_{k=0}^{n-1}\lvert y(t_{k+1})-y(t_k) \rvert\leqslant\\
    \leqslant \mathop{\mathrm{\mbox{\Large{V}}}}_a^b(x) + \mathop{\mathrm{\mbox{\Large{V}}}}_a^b(y).\end{gathered}$$
    Так как это неравенство верно для любого разбиения отрезка $[a;b]$,
    то и
    $\mathop{\mathrm{\mbox{\Large{V}}}}_a^b(x+y)\leqslant \mathop{\mathrm{\mbox{\Large{V}}}}_a^b(x) + \mathop{\mathrm{\mbox{\Large{V}}}}_a^b(y)$.

-   если $x$ --- Ф.О.В., то
    $\mathop{\mathrm{\mbox{\Large{V}}}}_a^c(x) + \mathop{\mathrm{\mbox{\Large{V}}}}_c^b(x) = \mathop{\mathrm{\mbox{\Large{V}}}}_a^b(x)$
    для любого $c\in (a;b)$.

    Доказательство. Пусть $T=\{t_i\}_{i=0}^n$ --- разбиение $[a;b]$ и
    $c\in [t_k,t_{k+1}]$. В силу неравенства
    $\lvert x(t_{k+1})-x(t_k) \rvert\leqslant\lvert x(t_{k+1})-x(c) \rvert+\lvert x(c)-x(t_k) \rvert$
    получаем
    $$\nu(T)\leqslant\nu(T\cup\{c\})=\nu(\{t_i\}_{i=0}^k \cup \{c\})+\nu(\{c\}\cup\{t_i\}_{i=k+1}^n)\leqslant
    \mathop{\mathrm{\mbox{\Large{V}}}}_a^c(x)+\mathop{\mathrm{\mbox{\Large{V}}}}_c^b(x),$$
    откуда
    $\mathop{\mathrm{\mbox{\Large{V}}}}_a^b(x)\leqslant \mathop{\mathrm{\mbox{\Large{V}}}}_a^c(x)+\mathop{\mathrm{\mbox{\Large{V}}}}_c^b(x)$.
    Обратно, пусть $\nu(\{t_i\}_{i=0}^n)$ и $\nu(\{t_j'\}_{j=0}^m)$ ---
    вариационные суммы функции $x$ на отрезках $[a,c]$ и $[c,b]$
    соответственно. Тогда $\nu(\{t_i\}_{i=0}^n \cup \{t_j'\}_{j=0}^m)$
    --- вариационная сумма для $x$ на всем отрезке $[a;b]$. Отсюда
    получаем неравенство
    $$\nu(\{t_i\}_{i=0}^n) + \nu(\{t_j'\}_{j=0}^m) = 
    \nu(\{t_i\}_{i=0}^n \cup \{t_j'\}_{j=0}^m) \leqslant \mathop{\mathrm{\mbox{\Large{V}}}}_a^b (x),$$
    откуда
    $\mathop{\mathrm{\mbox{\Large{V}}}}_a^c(x)+\mathop{\mathrm{\mbox{\Large{V}}}}_c^b(x)\leqslant \mathop{\mathrm{\mbox{\Large{V}}}}_a^b(x)$.

-   если $x$ -- Ф.О.В. на $[a;b]$, то $x$ ограничена на $[a;b]$.

Символом $V[a;b]$ будем обозначать множество всех вещественнозначных
функций ограниченной вариации, заданных на отрезке $[a;b]$.

Из свойств вариации следует, что
$\mathop{\mathrm{\mbox{\Large{V}}}}_a^b$ --- норма на линейном
пространстве $E=\left\lbrace x\in V[a;b] : x(a)=0 \right\rbrace$.

Непрерывная Ф.О.В.: $x(t)=\sin t$, $t\in [0;3\pi]$.
$\mathop{\mathrm{\mbox{\Large{V}}}}_0^{3\pi}(x)=6$.

Разрывная Ф.О.В.: $x(t)=\mathop{\mathrm{sgn}}t$, $t\in [-1;1]$.
$\mathop{\mathrm{\mbox{\Large{V}}}}_{-1}^1(x)=2$.

Непрерывная функция, не являющаяся Ф.О.В.:
$x(t)=t\cdot\cos \dfrac{\pi}{2t}$, $t\in (0;1]$ и $x(0)=0$. Если
разбиение $T$ --- это точки
$$0<\frac{1}{2n}<\frac{1}{2n-1}<\ldots <\frac{1}{3}<\frac{1}{2}<1,$$ то
соответствующая этому разбиению вариационная сумма будет равна
$$1+\frac{1}{2}+\ldots +\frac{1}{n}, \text{ откуда } \mathop{\mathrm{\mbox{\Large{V}}}}_0^1(x)=+\infty.$$

Разрывная функция, не являющаяся Ф.О.В.: функция Дирихле на отрезке
$[0;1]$. Если в качестве точек $t_2, t_4,\ldots , t_{2n-2}$ разбиения
$T$ брать рациональные числа, а в качестве $t_1, t_3,\ldots , t_{2n-1}$
--- иррациональные, то $\nu(T)=2n$, откуда
$\mathop{\mathrm{\mbox{\Large{V}}}}_0^1(x)=+\infty$.

### Интеграл Римана--Стилтьеса

Пусть $x$ и $g$ --- вещественнозначные функции, заданные на отрезке
$[a;b]$ и $T=\{t_k\}_{k=0}^n$ --- разбиение $[a;b]$. Выберем точки
$\xi_k\in [t_k,t_{k+1}]$ и составим сумму
$\sigma(T) = \sum_{k=0}^{n-1} x(\xi_k)(g(t_{k+1})-g(t_k))$.

Число
$\lambda (T)=\max\left\lbrace \lvert t_{k+1}-t_k \rvert : k=0,\ldots, n-1 \right\rbrace$
будем называть *мелкостью* разбиения $T$.

Если существует предел $$\lim_{\lambda(T)\to 0} \sigma(T),$$ не
зависящий от выбора точек $\xi_k$, то он называется *интегралом
Римана--Стилтьеса от функции $x$ по функции $g$ на отрезке $[a;b]$* и
обозначается $$\int_a^b x(t)dg(t).$$

Если $g(t)=t$, то интеграл Римана--Стилтьеса совпадает с обычным
интегралом Римана от функции $x$ по отрезку $[a;b]$.

Свойства интеграла Римана--Стилтьеса:

(1) если существуют $\alpha\int_a^b x(t)dg(t)$ и
    $\beta\int_a^b y(t)dg(t)$, то
    $$\int_a^b (\alpha x(t)+\beta y(t))dg(t) = \alpha\int_a^b x(t)dg(t) + \beta\int_a^b y(t)dg(t);$$

(2) если существуют $\alpha\int_a^b x(t)dg(t)$ и
    $\beta\int_a^b x(t)dh(t)$, то
    $$\int_a^b x(t)d(\alpha g(t)+\beta h(t)) = \alpha\int_a^b x(t)dg(t) + \beta\int_a^b x(t)dh(t);$$

(3) если существует $\int_a^b x(t)dg(t)$, то
    $$\int_a^b x(t)dg(t) = \int_a^c x(t)dg(t) + \int_c^b x(t)dg(t)$$ для
    любой точки $c\in [a;b]$. Обратное неверно, как показывает следующий
    пример: пусть $[a;b]=[-1;1]$ и $x=\chi_{(0;1]}$, $g=\chi_{[0;1]}$.
    Тогда $\int_{-1}^0 x(t)dg(t) = \int_0^1 x(t)dg(t) = 0$. Теперь
    рассмотрим число $\delta >0$ и такое разбиение $T$ отрезка $[-1;1]$,
    что $-1 < t_k < 0 < t_{k+1}<1$ и $\lambda (T)<\delta$. Тогда
    $$\int_{-1}^1 x(t)dg(t) = x(\xi_k)=\left\{
    \begin{array}{ll}
    0, & \text{если }\xi_k<0;  \\ 
    1, & \text{если }\xi_k>0.
    \end{array}\right.$$

(4) интегралы $\int_a^b x(t)dg(t)$ и $\int_a^b g(t)dx(t)$ либо
    одновременно существуют, либо одновременно не существуют, причём,
    если они оба существуют, то
    $$\int_a^b x(t)dg(t) + \int_a^b g(t)dx(t) = x(t)g(t)\vert_a^b$$
    (формула интегрирования по частям).

    Доказательство. Рассмотрим интегральную сумму для
    $\int_a^b x(t)dg(t)$: $$\begin{split}
    \sum_{k=0}^{n-1} x(\xi_k)&(g(t_{k+1})-g(t_k)) =\\
    =&\sum_{k=0}^{n-1} x(\xi_k)g(t_{k+1}) - \sum_{k=0}^{n-1} x(\xi_k)g(t_k)=\\
    =&\sum_{k=1}^{n} x(\xi_{k-1})g(t_k) - \sum_{k=0}^{n-1} x(\xi_k)g(t_k)=\\
    =&\sum_{k=1}^{n-1} g(t_k)(x(\xi_{k-1})-x(\xi_k))+
    x(\xi_{n-1})g(t_n)-x(\xi_0)g(t_0)=\\
    =&\sum_{k=1}^{n-1} g(t_k)(x(\xi_{k-1})-x(\xi_k))+\\
    +&g(t_0)(x(t_0)-x(\xi_0)) + g(t_n)(x(\xi_{n-1}))-x(t_n))+\\
    +&\underbrace{x(t_n)g(t_n)-x(t_0)g(t_0)}_{=x(b)g(b)-x(a)g(a) = x(t)g(t)\vert_a^b}
    \end{split}$$

[\[thr\_jordan\]]{#thr_jordan label="thr_jordan"} Если $g$ --- Ф.О.В. на
$[a;b]$, то $g=u-v$, где $u$ и $v$ --- неубывающие на $[a;b]$ функции.

Рассмотрим функцию $u(t)=\mathop{\mathrm{\mbox{\Large{V}}}}_a^t (g)$ для
каждого $t\in [a;b]$. Функция $u$ --- неубывающая на $[a;b]$, так как
если $t_1>t_2$, то
$$u(t_1)=\mathop{\mathrm{\mbox{\Large{V}}}}_a^{t_1} (g)= \mathop{\mathrm{\mbox{\Large{V}}}}_a^{t_2}(g)+\mathop{\mathrm{\mbox{\Large{V}}}}_{t_2}^{t_1}(g)\geqslant \mathop{\mathrm{\mbox{\Large{V}}}}_a^{t_2}(g)=u(t_2).$$

Осталось показать, что функция $v=u-g$ неубывающая. Пусть $t_1 > t_2$.
$$v(t_1)-v(t_2) = u(t_1)-u(t_2) - g(t_1) +g(t_2) = 
\mathop{\mathrm{\mbox{\Large{V}}}}_{t_2}^{t_1} (g) - (g(t_1)-g(t_2))\geqslant 0.$$

[\[exist\_int\_RS\]]{#exist_int_RS label="exist_int_RS"} Если $x$
непрерывна на $[a;b]$ и $g$ --- Ф.О.В. на $[a;b]$, то
$\int_a^b x(t)dg(t)$ существует.

Сначала докажем эту теорему для случая, когда функция $g$ является
неубывающей. Пусть $T$ --- какое-нибудь разбиение отрезка $[a;b]$.
Рассмотрим нижнюю и верхнюю суммы Дарбу: $$\begin{aligned}
s(T) &= \sum_{k=0}^{n-1} m_k(g(t_{k+1})-g(t_k)), \text{ где } m_k = \min_{t\in [t_k,t_{k+1}]} x(t);\\
S(T) &= \sum_{k=0}^{n-1} M_k(g(t_{k+1})-g(t_k)), \text{ где } M_k = \max_{t\in [t_k,t_{k+1}]} x(t).\end{aligned}$$

Очевидно, что $s(T)\leqslant\sigma(T)\leqslant S(T)$. Убедимся, что
какие бы два разбиения $T_1$ и $T_2$ отрезка $[a;b]$ мы не взяли, всегда
будет $s(T_1)\leqslant S(T_2)$. Для этого рассмотрим разбиение
$T_3 = T_1\cup T_2$. Тогда
$s(T_1)\leqslant s(T_3)\leqslant S(T_3)\leqslant S(T_2)$. Таким образом,
существует
$\sup\left\lbrace s(T) \mid T \text{ --- разбиение } [a;b] \right\rbrace\stackrel{\text{ об.}}{=}J$.

Зафиксируем какое-либо разбиение $T=\{t_k\}_{k=0}^n$ отрезка $[a;b]$. Из
неравенств $s(T)\leqslant J\leqslant s(T)$ и
$s(T)\leqslant\sigma(T)\leqslant S(T)$ следует, что
$$\lvert J-\sigma(T) \rvert\leqslant S(T)-s(T)=\sum_{k=0}^{n-1} (M_k-m_k)(g(t_{k+1})-g(t_k)).$$

Пусть $\varepsilon>0$. В силу равномерной непрерывности функции $x$
найдётся такое $\delta >0$, что
$\lvert x(t')-x(t'') \rvert<\varepsilon/\mathop{\mathrm{\mbox{\Large{V}}}}_a^b(g)$,
если $\lvert t'-t'' \rvert<\delta$. Значит, если $T$ --- такое разбиение
$[a;b]$, что $\lambda(T)<\delta$, то
$$\lvert J-\sigma(T) \rvert\leqslant \sum_{k=0}^{n-1} (M_k-m_k)(g(t_{k+1})-g(t_k))<\sum_{k=0}^{n-1}
\frac{\varepsilon}{\mathop{\mathrm{\mbox{\Large{V}}}}_a^b(g)}\cdot(g(t_{k+1})-g(t_k)) = \varepsilon.$$
Итак, теорема доказана для случая, когда функция $g$ неубывающая.

Докажем теперь теорему в общем случае. По функцию $g$ можно представить
в виде разности $u-v$ неубывающих функций. Тогда интегралы
$\int_a^b x(t)du(t)$ и $\int_a^b x(t)dv(t)$ по доказанному ранее
существуют, а по второму свойству интеграла Римана--Стилтьеса существует
и интеграл $\int_a^b x(t)d(u(t)-v(t)) = \int_a^b x(t)dg(t)$.

Если $x$ --- Ф.О.В. на $[a;b]$, а $g$ непрерывна на $[a;b]$, то интеграл
$\int_a^b x(t)dg(t)$ существует.

Следует из свойства (4) интеграла Римана--Стилтьеса.

Если $x\in C[a;b]$, а $g$ --- Ф.О.В. на $[a;b]$, то
*$$\left\lvert \int_a^b x(t)dg(t) \right\rvert\leqslant \lVert x \rVert\cdot  \mathop{\mathrm{\mbox{\Large{V}}}}_a^b(g).$$*

$$\begin{split}
\lvert \sigma(T) \rvert &= \lvert \sum_{k=0}^{n-1} x(\xi_k)(g(t_{k+1})-g(t_k)) \rvert\leqslant\\
&\leqslant\sum_{k=0}^{n-1} \lvert x(\xi_k) \rvert\cdot\lvert (g(t_{k+1})-g(t_k)) \rvert\leqslant\\
&\leqslant\lVert x \rVert\cdot\sum_{k=0}^{n-1}\lvert (g(t_{k+1})-g(t_k)) \rvert\leqslant\lVert x \rVert\cdot\mathop{\mathrm{\mbox{\Large{V}}}}_a^b(g).
\end{split}$$

Пусть $x\in C[a;b]$ и $g(t)=\left\{
\begin{array}{ll}
\alpha, & \text{если }t\in[a,c);  \\ 
\beta, & \text{если }t\in(c,b];  \\ 
\gamma, & \text{если }t=c.
\end{array}\right.$\
Тогда
$\sigma(T) = \sum_{k=0}^{n-1} x(\xi_k)(g(t_{k+1})-g(t_k)) = x(\xi_k)\cdot(\beta-\alpha)\to x(c)\cdot(\beta-\alpha)$.
Таким образом, $\int_a^b x(t)dg(t) = x(c)\cdot (g(c+0)-g(c-0))$.

Пусть $x\in C[a;b]$ и $g(t)=\left\{
\begin{array}{ll}
\alpha, & \text{если }t\in[a;b);  \\ 
\beta, & \text{если }t=b.
\end{array}\right.$\
Тогда
$\sigma(T) = x(\xi_{n-1})(g(b)-g(t_{n-1}))\to x(b)\cdot(\beta-\alpha)$.
Таким образом, $\int_a^b x(t)dg(t) = x(b)\cdot (g(b)-g(b-0))$.

Если $x$ непрерывна на $[a;b]$, $g$ --- Ф.О.В. на $[a;b]$ и всюду на
интервале $(a;b)$ существует $g'$, то
$(\text{RS})\int_a^b x(t)dg(t) = (\text{R})\int_a^b x(t)g'(t)dt$ если
последний интеграл существует.

Пусть $T$ --- разбиение $[a;b]$. По теореме Лагранжа о промежуточном
значении найдутся такие точки $\xi_k\in [t_k,t_{k+1}]$, что
$g(t_{k+1})-g(t_k) = g'(\xi_k)(t_{k+1}-t_k)$. Тогда
$$\sigma(T) = \sum_{k=0}^{n-1} x(\xi_k)(g(t_{k+1})-g(t_k))=
\sum_{k=0}^{n-1} x(\xi_k)g'(\xi_k)(t_{k+1}-t_k).$$

### Общий вид функционала на пространстве $C[a;b]$ {#общий-вид-функционала-на-пространстве-cab}

Формула $f(x)=\int_a^b x(t)dg(t)$, где $g$ --- Ф.О.В. на $[a;b]$,
определяет линейный ограниченный функционал на пространстве $C[a;b]$,
причём
$\lVert f \rVert\leqslant \mathop{\mathrm{\mbox{\Large{V}}}}_a^b(g)$.
Для каждого функционала $f\in C^\ast [a;b]$ найдётся такая Ф.О.В. $g$,
что $g(a)=0$ и $f(x) = \int_a^b x(t)dg(t)$.

Линейность следует из первого свойства интеграла Римана--Стилтьеса:
$$\begin{gathered}
f(\alpha x+\beta y) = \int_a^b (\alpha x(t)+\beta y(t))dg(t) =\\
=\alpha\int_a^b x(t)dg(t) + \beta\int_a^b y(t)dg(t) = \alpha f(x)+\beta f(y).\end{gathered}$$

Ограниченность вытекает из второго следствия из :

$$\left\lvert f(x) \right\rvert = \left\lvert \int_a^b x(t)dg(t) \right\rvert\leqslant \lVert x \rVert\cdot\mathop{\mathrm{\mbox{\Large{V}}}}_a^b(g), \text{ откуда } \lVert f \rVert\leqslant \mathop{\mathrm{\mbox{\Large{V}}}}_a^b(g).$$

Пусть теперь $f$ --- линейный ограниченный функционал на пространстве
$C[a;b]$. Рассмотрим банахово пространство $M[a;b]$ всех ограниченных на
$[a;b]$ функций с нормой
$\lVert x \rVert = \sup_{t\in [a;b]}\lvert x(t) \rvert$. Очевидно, что
$C[a;b]$ --- подпространство в $M[a;b]$. Тогда по функционал $f$
продолжается на все пространство $M[a;b]$ до линейного непрерывного
функционала $\tilde{f}$, причём
$\lVert f \rVert = \lVert \tilde{f} \rVert$.

Далее для каждого $t\in (a;b)$ рассмотрим функции $u_t\in M[a;b]$,
определенные формулой $u_t(s)=\left\{
\begin{array}{ll}
1, & \text{если }s\in[a,t);  \\ 
0, & \text{если }s\in[t,b].
\end{array}\right.$ и функции $u_a\equiv 0$ и $u_b\equiv 1$.

Определим функцию $g$ на $[a;b]$ следующим образом:
$g(t)=\tilde{f}(u_t)$ для каждого $t\in [a;b]$ и докажем, что она имеет
ограниченную вариацию. Для этого оценим вариационную сумму:
$$\begin{gathered}
\nu(T)=\sum_{k=0}^{n-1}\left\lvert g(t_{k+1})-g(t_k) \right\rvert = \sum_{k=0}^{n-1}\varepsilon_k \left(g(t_{k+1})-g(t_k)\right) = \\
=\sum_{k=0}^{n-1}\varepsilon_k \left( \tilde{f}(u_{t_{k+1}})-\tilde{f}(u_{t_k})\right)  = 
\tilde{f}\left( \sum_{k=0}^{n-1}\varepsilon_k \left(u_{t_{k+1}}-u_{t_k}\right) \right)\leqslant\\
\leqslant\lVert \tilde{f} \rVert\cdot\left\lVert \sum_{k=0}^{n-1}\varepsilon_k \left(u_{t_{k+1}}-u_{t_k} \right) \right\rVert\leqslant\lVert \tilde{f} \rVert.\end{gathered}$$

Рассмотрим теперь произвольную функцию $x\in C[a;b]$. Пусть
$T=\{t_k\}_{k=0}^n$ --- \<\<равномерное\>\> разбиение $[a;b]$, то есть
такое, что $t_{k+1}-t_k = (b-a)/n$ для всех $k$. Теперь для каждого
$n\in\mathbb{N}$ определим \<\<ступенчатую\>\> функцию
$y_n(t) = \sum_{k=0}^{n-1} x(t_k) \left(u_{t_{k+1}}-u_{t_k}\right)$ и
докажем, что последовательность $\{y_n\}_{n=1}^\infty$ равномерно
сходится к $x$ на отрезке $[a;b]$. Действительно, пусть $\varepsilon>0$.
Из равномерной непрерывности функции $x$ следует, что найдётся такое
$\delta >0$, что $\lvert x(t')-x(t'') \rvert<\varepsilon$, если
$\lvert t'-t'' \rvert<\delta$. Теперь найдём такое $n_0$, что
$(b-a)/n_0<\delta$. Тогда при всех $n\geqslant n_0$ на каждом из
отрезков $[t_k,t_{k+1}]$ будет выполняться неравенство
$\left\lvert y_n(t)-x(t) \right\rvert = 
\left\lvert x(t_k)-x(t) \right\rvert<\varepsilon$. Следовательно,
$y_n\rightrightarrows x$ на всем отрезке $[a;b]$. Тогда, в силу
непрерывности функционала $\tilde{f}$ будем иметь
$\tilde{f}(y_n)\xrightarrow[n\to\infty]{}\tilde{f}(x)$. C другой
стороны, $$\begin{gathered}
\tilde{f}(y_n)=\sum_{k=0}^{n-1} x(t_k) \left(\tilde{f}(u_{t_{k+1}})-\tilde{f}(u_{t_k})\right) = \\
= \sum_{k=0}^{n-1} x(t_k) \left(g(t_{k+1})-g(t_k)\right)\xrightarrow[n\to\infty]{}\int_a^b x(t)dg(t),\end{gathered}$$
откуда для любой функции $x\in C[a;b]$ получаем равенство
$\tilde{f}(x) = f(x) = \int_a^b x(t)dg(t)$.