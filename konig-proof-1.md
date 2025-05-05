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

$$q_k = q_{k-1}a_k + q_{k-2} \ge q_{k-1} + q_{k-2}$$

$$q_0=1$$
$$q_1 = a_1 \ge 1$$
$$q_2 \ge q_{1} + q_{0} = 1 + 1 = 2$$
$$q_3 \ge q_{2} + q_{1} = 2 + 1 = 3$$
$$q_4 \ge q_{3} + q_{2} = 3 + 2 = 5$$
$$...$$

$$q_k \ge q_{k-1} + q_{k-2}$$
$$\frac{q_k}{q_{k-1}} \ge 1 + \frac{q_{k-2}}{q_{k-1}}$$
$$\varphi_k = \frac{q_{k-1}}{q_{k-2}}$$
$$\varphi_{k+1} \ge 1 + \frac{1}{\varphi_{k}}$$
$$\varphi_{k+1}\varphi_{k} \ge \varphi_{k} + 1$$
$$\varphi_{k+1}\varphi_{k} - \varphi_{k} - 1 \ge 0$$

$$k=3: \frac{q_3}{q_{2}} \ge 1 + \frac{q_{1}}{q_{k-1}}$$