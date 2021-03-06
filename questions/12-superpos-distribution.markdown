---
title: "Функции распределения функций случайных величин"
---
 Функции распределения функций случайных величин ##

### Def. (Борелевская функция) ###
Борелевской называется измеримая функция вида $g : (\RR^n, \BB^n)\mapsto (\RR^m,\BB^m)$.
То есть функция, относительно которой прообразами борелевских множеств являются борелевские множества.

### Def. (Борелевская фунция от случайной величины) ###
Пусть $X = (X_1, \ldots, X_n)$ --- r.v. на $(\Omega, \FF, \pr)$.
${\Psi_j, j=\overline{1,k}}$ --- борелевские функции ${\Psi_j : X(\Omega)\mapsto\RR}$.
${\Psi = (\Psi_1, \ldots, \Psi_k)}$,
${\Psi : X(\Omega)\mapsto\Gamma, \quad \Gamma\subset\RR^k}$ --- отображение из области $X(\Omega)$ значений r.v. $X$
в область $k$-мерного вещественного пространства.

$Y = (Y_1, \ldots, Y_k), \quad Y_j = \Psi_j(X)$ --- случайная величина $Y: \Omega\mapsto\Gamma$
(доказать: композиция борелевской ф-ии и случайной величины есть случайная величина).

Пусть $F_X$ --- функция распределения r.v. $X$.

### Задача: найти функцию $F_Y$ распределения $Y$ ###

$$F_Y(y) = \pr \{Y(\omega) \leq y\} = \pr \{ \Psi(X(\omega)) \leq y\}$$

Будем искать функцию распределения $F_Y$ по заданной плотности $f_X$.

1.  Пусть $k=n=1$.
    
    $X$ --- непрерывная r.v., $f_X$ --- плотность.
    $Y = \Psi(X)$.
    
    Найдём $F_Y$:
    $F_Y(y) = \pr\{\Psi(X)\leq y\} = \int_{\{x: \psi(x) \leq y\}} f_X(x) \dd x$

2.  $1 \leq k \leq n$
    
    $X = (X_1, \ldots, X_n)$
    $f_X : X(\Omega)\mapsto\RR_+$ --- плотность.

    $Y = (Y_1, \ldots, Y_k) = (\Psi_1(X), \ldots, \Psi_k(X)$ --- r.v.

    $F_Y(y) = \pr(\Psi(X)\leq y) = \idotsint_{\{ x: \Psi(x) \leq y \}} f_X(x) \dd x$,
    где ${x=(x_1, \ldots, x_n)}, {y=(y_1,\ldots,y_n)}, {\dd x = \dd x_1 \ldots \dd x_n}$
