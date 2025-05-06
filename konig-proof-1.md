---
mainfont: DejaVuSerif
sansfont: DejaVuSans
monofont: DejaVuSansMono
mathfont: latinmodern-math.otf
papersize: a4
lang: RU-ru
pagestyle: empty
margin-left: 20mm
margin-right: 20mm
margin-top: 20mm
margin-bottom: 20mm
---

Вопрос по задачам: "4 Теорема Валена" и "5 Доказать формулу Перрона". В формулах, которые нужно доказать, присутствует расстояние до ближайшего целого от выражения $\left\Vert q_n\xi \right\Vert$ (знаменатель подходящей дроби $q_n$ умножить на число $\xi$). В книге Хинчин "Цепные дроби" есть теоремы с доказательствами нужных мне формул, но там вместо расстояния до ближайшего целого стоит модуль расстояния между числом $\xi$ и подходящей дробью $\frac{p_n}{q_n}$.

Докажем формулу:
$$\begin{equation}
q_n\left|{\xi - \frac{p_n}{q_n}}\right| = \left\Vert q_n\xi \right\Vert
\end{equation}$$

Доказательство
$$\begin{align*}
q_0\left|{\xi - \frac{p_0}{q_0}}\right| 
= 1\cdot\left|[a_0;r_1] - \frac{a_0}{1}\right| 
= \left|a_0 + \cfrac{1}{r_1} - a_0\right| 
= \frac{1}{r_1}
\end{align*}$$
$$\begin{align*}
\left\Vert q_0\xi \right\Vert = \left\Vert 1\cdot\xi \right\Vert = \left\Vert \xi \right\Vert
\end{align*}$$

Пример: $\xi=\frac{3}{11}$. Представление $\xi$ в виде цепной дроби:
$$\begin{align*}
\xi = \frac{3}{11} &= [0;3,1,2] =\\
                   &= 0+\cfrac{1}{3+\cfrac{1}{1+\cfrac{1}{2}}}
\end{align*}$$

$$\begin{align*}
\cfrac{1}{2} = -1 + \cfrac{1}{-3 + \cfrac{1}{-0 + \cfrac{3}{11}}} = [-1;-3,0,\frac{3}{11}]
\end{align*}$$

Подходящие дроби и проверка формулы (1):
$$\begin{align*}
\frac{p_0}{q_0} &= \frac{0}{1}:\quad &1\cdot\left|{\frac{3}{11} - \frac{0}{1}}\right| = \left\Vert 1\cdot\frac{3}{11}\right\Vert = \frac{3}{11}\\
\frac{p_1}{q_1} &= \frac{1}{3}:\quad &3\cdot\left|{\frac{3}{11} - \frac{1}{3}}\right| = \left\Vert 3\cdot\frac{3}{11}\right\Vert = \frac{2}{11}\\
\frac{p_2}{q_2} &= \frac{1}{4}:\quad &4\cdot\left|{\frac{3}{11} - \frac{1}{4}}\right| = \left\Vert 4\cdot\frac{3}{11}\right\Vert = \frac{1}{11}\\
\frac{p_3}{q_3} &= \frac{3}{11}:\quad &11\cdot\left|{\frac{3}{11} - \frac{3}{11}}\right| = \left\Vert 11\cdot\frac{3}{11}\right\Vert = 0
\end{align*}$$