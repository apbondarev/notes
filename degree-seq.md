---
mainfont: "Cactus Classical Serif"
mathfont: latinmodern-math.otf
papersize: a4
lang: RU-ru
pagestyle: empty
margin-left: 20mm
margin-right: 20mm
margin-top: 20mm
margin-bottom: 20mm
---

Пусть $X_j$ - случайная величина равная количеству вершин со степенью $j$ в случайном графе.

Пусть $Y_2$ - случайная величина равная количеству вершин в случайном графе со степенью не менее 2-х. 

$$Y_2 = X_2 + X_3 + \dots + X_{n-1}$$

По свойству линейности мат ожидания:
$$E(Y_2)=\sum\limits_{j=2}^{n-1}E(X_j)$$

Когда вершина имеет степень $j$? Рассмотрим произвольную вершину. Количество ее соседей равно $n-1$. Чтобы эта вершина имела степень $j$ она вершина должна быть соединена ребрами с $j$ соседними вершинами, и должны отсутствовать ребра с остальными $n-1-j$ вершинами. Количество способов выбрать $j$ вершин среди $n-j$ равно $C_{n-1}^j$. Вероятность, что данная вершина имеет степень $j$ не превосходит суммы вероятностей по всем способам выбрать $j$ соседей:
$$P(deg(v_i)=j) \leq C_{n-1}^j p^j (1-p)^{n-1-j}$$

Мат ожидание случайной величины $X_j$ равно сумме мат ожиданий случайных величин индикаторов $X_{i,j}$ (1 - если степень $i$-й вершины графа равна $j$; 0 - иначе):
$$E(X_j) = \sum\limits_{i=1}^{n}\:X_{i,j} \leq \sum\limits_{i=1}^{n} C_{n-1}^j\:p^j\:(1-p)^{n-1-j}$$

Оценим сверху: 
$$\begin{split}
0 < \;p < 1\\
-1 < \;p-1 < 0\\
0 < \;1-p < 1\\
(1-p)^{n-1-j} < 1&
\end{split}$$


Оценим сверху: $C_{n-1}^j= \frac{(n-1)\cdots(n-1-j+1)}{j!} = \frac{(n-1)\cdots(n-j+1)(n-j)}{j!} \leq \frac{n(n-1)\cdots(n-j+1)}{j!} = C_{n}^j$

Получаем неравенство: $E(X_j) \leq \sum\limits_{i=1}^{n} C_{n-1}^j\:p^j = n\;C_{n-1}^j\:p^j \leq n\,C_n^j\:p^j$

Мат ожидание количества вершин степени не менее 2-х:
$$E(Y_2) \leq n\sum\limits_{j=2}^{n-1} C_{n}^j\:p^j$$

Используем оценку для $C_{n}^j = \frac{n(n-1)\cdots(n-j+1)}{j!} \leq \frac{n^j}{j!}$
$$E(Y_2) \leq n\sum\limits_{j=2}^{n-1} C_{n}^j\:p^j \leq n\sum\limits_{j=2}^{n-1} \frac{(n\,p)^j}{j!}$$

Почему справедливо неравенство $n\sum\limits_{j=2}^{n-1} \frac{(n\,p)^j}{j!} \leq \sum\limits_{j=2}^{\infty} \frac{(n\,p)^j}{j!}$

В итоге получаем цепочку неравенств:
$$E(Y_2) = \sum\limits_{j=2}^{n-1}E(X_j) \leq n\sum\limits_{j=2}^{n-1} C_{n}^j\:p^j \leq n\sum\limits_{j=2}^{n-1} \frac{(n\,p)^j}{j!}$$

Доказательство, что 
$$n\sum\limits_{j=2}^{n-1} \frac{(n\,p)^j}{j!} < \sum\limits_{j=2}^{\infty} \frac{(n\,p)^j}{j!}$$

Левая часть неравенства. Используем $j!\ge2^{j-1}$
$$
n\sum\limits_{j=2}^{n-1} \frac{(n\,p)^j}{j!} 
\le n\sum\limits_{j=2}^{n-1} \frac{(n\,p)^j}{2^{j-1}}
= 2n\sum\limits_{j=2}^{n-1} \left(\frac{n\,p}{2}\right)^j 
$$

Здесь правая часть это геометрическая прогрессия с коффициентом меньше $\frac{np}{2} < 1$, поэтому сумма 

Если $p=o(n^{-3/2})$, то $np=o(n^{-1/2})$. Отсюда следует, что начиная с некоторого $n>n_0$ будет выполняться неравенство $\frac{n\,p}{2} < 1$. Поэтому сумма не превосходит:

$$
2n \frac{1}{1-\frac{n\,p}{2}} 
\le \frac{2n}{1-\frac{n\,p}{2}} 
= \frac{(np)^2}{2} \frac{n}{1-\frac{n\,p}{2}}
$$

Правая часть неравенства (используем неравенство $\frac{n\,p}{2} < 1$):
$$
\sum\limits_{j=2}^{\infty} \frac{(n\,p)^j}{j!} 
= e^{np} - 1 - \frac{np}{1!} 
> \frac{(np)^2}{2!} + \frac{(np)^3}{3!}
= \frac{(np)^2}{2} \left(1 + \frac{np}{3}\right)
$$

Теперь сравним левую и правую часть неравенства:
$$
\frac{(np)^2}{2} \frac{n}{1-\frac{n\,p}{2}} \langle?\rangle \frac{(np)^2}{2} \left(1 + \frac{np}{3}\right)\\
$$
$$
\frac{n}{1-\frac{n\,p}{2}} \langle?\rangle 1 + \frac{np}{3}
$$



Если $p=o(n^{-3/2})$, то
$$\frac{n\cdot o(n^{-3/2})}{j!} = \frac{o(n^{-1/2})}{j!} = o(\frac{1}{\sqrt{n}}) \cdot \frac{1}{j!}$$

Обозначение $g(n) = o(\frac{1}{\sqrt{n}})$ означает, что $\lim\limits_{n\rightarrow\infty}(\sqrt{n} \cdot g(n)) = 0$

$$
\sum\limits_{j=2}^{n-1} \frac{(n\,p)^j}{j!} 
= \frac{1}{o(\sqrt{n})} \cdot \sum\limits_{j=2}^{n-1} \frac{1}{j!} 
\leq \frac{1}{o(\sqrt{n})} \sum\limits_{j=0}^{\infty} \frac{1}{j!} 
= \frac{1}{o(\sqrt{n})} \cdot e
= o(1)
$$
