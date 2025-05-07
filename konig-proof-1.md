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

### Теорема. Всякое наилучшее приближение второго рода есть подходящая дробь.

### Доказательство

Пусть дробь $\frac{a}{b}$ — есть наилучшее приближение второго рода числа 
$$\alpha = [a_0, a_1, a_2, ...],$$
подходящие дроби которого будем обозначать через $\frac{p_k}{q_k}$
Если бы было $\frac{a}{b} < a_0$, то на числовой прямой значения располагались в следующей последовательности $\frac{a}{b} < a_0 \le \alpha$ и мы имели бы неравенство:

$$\begin{align*}
\left|1\cdot\alpha - a_0\right| < \left|\alpha - \frac{a}{b}\right|
\end{align*}$$

Так как $b \ge 1$, то справедливы неравенства:
$$b\alpha \ge \alpha$$
$$\frac{a}{b} \le a$$

Отсюда следует, что: $\left|\alpha - \frac{a}{b}\right| \le \left|b\alpha - a\right|$ и
$$\left|1\cdot\alpha - a_0\right| < \left|b\alpha - a\right|$$

Таким образом, если бы было $\frac{a}{b} < a_0$, то приближение $\frac{a}{b}$ было бы хуже, чем приближение $\frac{a_0}{1}$. В таком случае $\frac{a}{b}$ не будет наилучшим приближением второго рода. Таким образом, $\frac{a}{b} \ge a_0$. Предположим противное: дробь $\frac{a}{b}$ не совпадает ни с одною из подходящих дробей. Тогда она должна либо быть заключенной между двумя подходящими дробями $\frac{p_{k-1}}{q_{k-1}}$ и $\frac{p_{k+1}}{q_{k+1}}$ одинаковой четности, либо быть больше чем $\frac{p_1}{q_1}$.

### Случай 1: дробь $\frac{a}{b}$ заключенной между двумя подходящими дробями $\frac{p_{k-1}}{q_{k-1}}$ и $\frac{p_{k+1}}{q_{k+1}}$ одинаковой четности
$$\begin{align*}
\left|\frac{a}{b} - \frac{p_{k-1}}{q_{k-1}}\right| 
= \left|\frac{a\,q_{k-1} - b\,p_{k-1}}{b\,q_{k-1}}\right| 
\ne 0 
\ge \frac{1}{b\,q_{k-1}}
\end{align*}$$

и
$$\begin{align*}
\left|\frac{a}{b} - \frac{p_{k-1}}{q_{k-1}}\right| 
< \left|\frac{p_{k}}{q_{k}} - \frac{p_{k-1}}{q_{k-1}}\right|
= \left|\frac{p_k\,q_{k-1} - q_k\,p_{k-1}}{q_k\,q_{k-1}}\right| 
= \frac{1}{q_k\,q_{k-1}}
\end{align*}$$

откуда
$$\begin{align*}
\frac{1}{b\,q_{k-1}} &< \frac{1}{q_k\,q_{k-1}}\\
\frac{1}{b} &< \frac{1}{q_k}
\end{align*}$$
$$\begin{align}
b &> q_k
\end{align}$$

С другой стороны дроби одинаковой четности находятся с одной стороны от числа $\alpha$ и с увеличением индекса приближаются к числу $\alpha$. Поэтому модуль разности $\left|\alpha - \frac{p_{k+1}}{q_{k+1}}\right|$ больше, чем $\left|\alpha - \frac{p_{k-1}}{q_{k-1}}\right|$. Так как дробь $\frac{a}{b}$ расположена между дробями $\frac{p_{k-1}}{q_{k-1}}$ и $\frac{p_{k+1}}{q_{k+1}}$. Это означает, что расстояние между $\frac{a}{b}$ и $\alpha$ больше, чем расстояние между $\frac{a}{b}$ и $\frac{p_{k+1}}{q_{k+1}}$:
$$\begin{align*}
\left|\alpha - \frac{a}{b}\right| 
\gt \left|\frac{p_{k+1}}{q_{k+1}} - \frac{a}{b}\right| 
= \left|\frac{b\,p_{k+1} - a\,q_{k+1}}{b\,q_{k+1}}\right| 
\neq 0
\geq \frac{1}{b\,q_{k+1}}
\end{align*}$$

Итак получили:
$$\left|\alpha - \frac{a}{b}\right| \gt \frac{1}{b\,q_{k+1}} $$
$$\begin{align}
\left|b\alpha - a\right| \gt \frac{1}{q_{k+1}}
\end{align}$$

Воспользуемся оценкой на расстояние между числом и последовательными дробями:
$$\left|\alpha - \frac{p_{k}}{q_{k}}\right| \leq \frac{1}{q_{k}q_{k+1}}$$

Умножив обе части этого неравенства на $q_{k}$ получим:
$$\begin{align}
\left|q_{k}\alpha - p_{k}\right| \leq \frac{1}{q_{k+1}}
\end{align}$$

Из цепочки неравенств (2) и (3) следует:
$$\begin{align}
\left|q_{k}\alpha - p_{k}\right| \lt \left|b\alpha - a\right|
\end{align}$$

В (1) было доказано неравенство $b \gt q_k$. Поэтому из (4) следует:
$$\begin{align}
\left|q_{k}\alpha - p_{k}\right| \lt \left|q_{k}\alpha - a\right|
\end{align}$$