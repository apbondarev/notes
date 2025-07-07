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

Пусть дробь $\frac{p}{q}$ представима в виде цепной дроби $[0; a_1, r_2]$. Где $r_2 = \frac{q'}{p'}$ несократимая дробь. Тогда

$$\frac{p}{q} = \cfrac{1}{a_1 + \cfrac{p'}{q'}} = \frac{q'}{a_1 q' + p'}$$

Если дробь $\frac{p}{q}$ несократима $(p,q)=1$, то 
$$p = q'$$
$$q = a_{1}q' + p'$$

Поиск пересечения $1/2$
$$x \in \left[1, \left[\frac{q+1}{2} \right] - 1\right]$$
$$y = 2 \left[\frac{q+1}{2} \right] - x - 1$$
$$\frac{\left[\frac{q+1}{2} \right]}{x} - 1 = \frac{1}{2}$$
$$\left[\frac{q+1}{2} \right] - x = \frac{x}{2}$$
$$\left[\frac{q+1}{2} \right] = \frac{3x}{2}$$

$$x = \frac{2}{3}\left[\frac{q+1}{2} \right]$$

Пример: пусть $q = 2^7 = 128$
$$x = \frac{2}{3}\left[\frac{128+1}{2} \right] = \frac{2}{3} \cdot 64 \notin \mathbb{N}$$

Поиск пересечения $1/3$
$$i=0,1,2,...$$
$$x = \left[\frac{q+1}{3} \right] - 2i - 1 $$
$$y = \left[\frac{q+1}{3} \right] + i$$
$$\frac{\left[\frac{q+1}{2} \right]}{x} - 1 = \frac{1}{2}$$
$$\left[\frac{q+1}{2} \right] - x = \frac{x}{2}$$
$$\left[\frac{q+1}{2} \right] = \frac{3x}{2}$$

$$x = \frac{2}{3}\left[\frac{q+1}{2} \right]$$
