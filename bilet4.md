###Билет 4
#####Решение УШ для линейного осциллятора, уровни энергии и волновые функции
Линейный осциллятор: $U(x) = \frac{1}{2}m\omega^2x^2$
$\hat H = \dfrac{p^2}{2m}+\dfrac{m\omega^2z^2}{2}$
$\dfrac{d^2\psi}{dx^2}+\dfrac{2m}{h^2}(E-\dfrac{m\omega^2x^2}{2})\psi=0$
Перейдем к безразмерным величинам
$\tilde{x}=\dfrac{x}{l},\quad\text{ где } l = \sqrt{\dfrac{\hbar}{m\omega}}-\text{ амплитуда колебаний}$

$\tilde E = \dfrac{E}{\hbar \omega} \qquad (1)$
При этом волновая функция $\psi(x)$ связана с безразмерной $\tilde\psi(\tilde x)$ соотношением
$\psi(x) = \dfrac{\tilde\psi(\frac{\tilde x}{l})}{\sqrt{l}}$
Тогда получим УШ в виде:
$\dfrac{d^2\psi}{d\tilde x^2}+\dfrac{2m}{h^2}(\tilde E-\tilde x^2)\psi=0$
Далее тильду опускаем.
При $x\to \pm\infty \text{ имеем }\dfrac{d^2\psi}{dx^2=x^2}\psi \quad\text{ т.е. }\quad \psi \to e^{\pm \frac{x^2}{2}}$. Поэтому ищем нормируемые, убывающие на бесконечности решения в виде
$\psi = e^{\frac{-x^2}{2}}v(x)$
где
$v''-2xv'+(2E-1)v=0$.
Ищем $v$ в виде ряда
$v = \sum\limits_{n=0}^{\infty}a_nx^n$
Возникающее таким образом уравнение
$\sum\limits_n x^n[(2E-1-2n)a_n+(n+1)(n+2)a_{n+2}]=0$
приводит к рекуррентному соотношению для коэффициентов
$a_{n+2}=\dfrac{2n+1-2E}{(n+1)(n+2)}a_n$.
Оно означает, что функция $v(x)$ сожержит слагаемые одинаковой четности. Условие
$\lim\limits_{n\to\infty}\dfrac{a_{n+2}}{a_n}=\dfrac{2}{n}\to 0$
обеспечивает сходимость ряда при всех $x$, но $v(x)\to e^{x^2}\text{ при } x\to \pm \infty$. Чтобы получить $\psi(x)\to 0\text{ при } x\to \pm\infty,$ необходимо ряд для $v(x)$ оборвать, положив
$2E = 2n +1$
В итоге получаем уровни энергии и нормированные волновые функции
$E_n = n+ \frac{1}{2}, \quad \psi_n(x)=\dfrac{e^{-\frac{x^2}{2}}}{\sqrt[4]{\pi}}\dfrac{H_n(x)}{\sqrt{n!2^n}}, \quad n = 0,1,2...$
из (1): $E = \hbar\omega(n+\frac{1}{2})-\text{ уровни энергии}\qquad (2) $
Здесь $H_n-$полиномы Эрмита:
$H_0(x)=1, \quad H_1(x)=2x, \quad H_{n+1}(x)-2nH_{n-1}(x)$
Отметим, что
$\psi_n(-x)=(-1)^n\psi_n(x)$
из (2): $E_0 = \dfrac{\hbar\omega}{2} = \dfrac{m\omega^2x^2}{2}$
$x_{stop}= \sqrt{\dfrac{E_0}{\hbar\omega}} = l (\text{для }n=0)$
###Билет 5
####Эрмитовы операторы
Оператор $\hat B$ называется **эрмитово сопряженным** к оператору $\hat A$, если для любых двух функций $\psi_1 \text{ и }\psi_2$ справедливо соотношением
$$\int dx \ \psi_1^* \hat A \psi_2 = \int dx \ (\hat B \psi_1)^* \psi_2.$$

Обозначим такой оператор $\hat B =\hat A^{\dagger}$. Если $\hat A = \hat A^{\dagger}$, т.е. оператор совпадает со своим эрмитово сопряженным, то он **эрмитово сопряженный** (или **самосопряженный**). Для эрмитова оператора
$$\int dx \ \psi_1^* \hat A \psi_2 = \int dx \ (\hat A \psi_1)^* \psi_2.$$
####Вещественность собственных значений
Собственные значения эрмитова оператора вещественны:
$$\hat A\psi_{\lambda}=\lambda\psi_{\lambda} \ \bigg | \cdot\psi_{\lambda}^* \Rightarrow \quad \int dx \ \psi_{\lambda}^* \hat A \psi_{\lambda} = \int dx \ (\hat A \psi_\lambda)^* \psi_{\lambda}.$$

Отсюда следует, что $\lambda = \lambda^* $

Среднее значение эрмитова оператора вещественно:
$$\bar A = \int\psi^* (x) \hat A \psi(x) dx = \int(\hat A^* \psi)^* \psi(x)dx = \int \hat A \psi^* \psi dx = \bar A $$

$$\bar A^* = \int \psi(x)\hat A^* \psi^* (x) = \int \psi(x)(\hat A\psi^* (x) )dx = \bar A^* $$

$\bar A = \bar A^* \Rightarrow \bar A \in \mathbb{R}$
####Ортогональность собственных функций
Собственные функции, отвечающие различным собственным значения эрмитова оператора, взаимно ортогональны. Действительно, домножив $\hat A\psi_{\lambda} = \lambda\psi_{\lambda} \text{ на } \psi_{\mu}^* \ \text{ а }, (\hat A\psi_{\mu})^* = \mu \psi_{\mu}^* \text{ на } \psi_{\lambda}$, и проинтегрировав, получим
$$\lambda\int dx \psi_{\mu}^* \psi_{\lambda} = \mu\int dx \psi_{\mu}^* \psi_{lambda},$$

т.е.
$$\int dx \psi_{\mu}^* \psi_{\lambda} = 0\text{ при } \mu \ne \lambda.$$

В случае вырождения можно выбрать собственные функции ортогональными и, использовать ортонормированную систему функций
$$\int dx \psi_m^* \psi_n = \delta_{mn}.$$
####Полнота собственных функций
Полнота системы собственных функций эрмитова оператора:
$$f(x) = \sum\limits_n a_n\psi_n(x); \quad a_n = \int dx' \psi_n^* (x') f(x'),$$

$$f(x)=\int dx' f(x')\sum\limits_n \psi_n(x)\psi_n^* (x').$$

Отсюда
$$\sum\limits_n \psi_n(x)\psi_n^* (x') = \delta(x-x').$$
