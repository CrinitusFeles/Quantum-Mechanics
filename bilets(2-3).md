
###Билет 2
####Свойства решений одномерного уравнения Шредингера
Введем УШ следующим образом. Пусть
<a name="abcd"></a>
$\begin{cases}\psi_p(x,t)= Ae^{i\frac{px}{\hbar}-i\frac{E_pt}{\hbar}}\qquad (1)\\
E_p = \dfrac{p^2}{2m}
\end{cases}$

$\dfrac{\partial }{\partial t}(1)\Rightarrow \dfrac{\partial }{\partial t}\psi(x,t)=\dfrac{-iE_p}{\hbar}\psi_p(x,t)=\dfrac{-ip^2}{2m\hbar}\psi_p(x,t)$
$\hat p^2 = -\hbar^2\dfrac{\partial^2 }{\partial x^2}$
$\dfrac{\partial }{\partial t}\psi(x,t)=\dfrac{i\hbar^2}{2m\hbar}\psi(x,t)\Rightarrow i\hbar\dfrac{\partial }{\partial t}\psi = -\dfrac{\hbar^2}{2m}\psi(x,t)$
В общем случае: $i\hbar\dfrac{\partial }{\partial t}\psi = \hat H\psi=(-\dfrac{\hbar^2}{2m}\Delta+U)\psi-$нестационарное УШ
В стационарном случае $\dfrac{\partial }{\partial t}$ нету $\Rightarrow \hat H \psi_n(x) = E_n\psi_n(x)$

***
Классическая функция Гамильтона
$H = \dfrac{p^2}{2m}+U(r)$
заменяется оператором Гамильтона
$\hat H = -\dfrac{\hbar^2}{2m}\Delta + U(r)$.
Собственная функция этого оператора с собственным значением $E_n$ удовлетворяет уравнению Шредингера
$\hat H \psi_n(x) = E_n\psi_n(x)$.
Решения этого уравнения ищутся в классе однозначных и непрерывных функций. В случае связанных состояний эти функции нормриуемы и поэтому $\psi_n(x)\to 0$ при $x\to \pm\infty$
**Свойтсва решений**
1)Для одномерного УШ движение финитно, следовательно спектр дискретный при $E<0$
2)**Осцилляционная теорема**
Волновая функция дискретного спектра $\psi_n(x)$, соответствующая $(n+1)$-му по величине собственному значению $E_n$, обращается в нуль(при конечных $x$) $n$ раз.
3)$\psi-$ основное состояние не имеет нулей
4)**Четные и нечетные решения**
Положим, что $U(x) = U(-x)-$ четная, тогда
$\hat H(x)\psi(x)=E\psi(x)$
$\hat H(-x)\psi(-x)=E\psi(-x)$
$\hat H(x)\begin{cases}\psi(x)=E\psi(x)\\
\psi(-x)=E\psi(x)
\end{cases}$
$\Downarrow\begin{cases}\psi''(x)=(E-U)\psi(x)\\
\psi''(-x)=(E-U)\psi(-x)
\end{cases}$
$\psi(x) = C\psi(-x)$
Меняем знак еще раз
$\psi(-x)=C\psi(x)$ и подставляем в (1)
$\psi(x)= C^2\psi(x)\Rightarrow C=\pm 1$
При симметричной относительно нуля яме уровни будут либо четные, либо нечетные.
5)**Дискретные уровни в одномерной задаче всегда невырождены**, т.е. каждому с.з. энергии соответствует единственная с.ф.
Доказательство от обратного: пусть $\psi_1(x)$ и $\psi_2(x)-$ две разные собственные функции $\hat H,$ отвечающие одному значению $E$. Тогда
$\dfrac{\psi_1''}{\psi_1}=\dfrac{2m}{\hbar^2}(U-E)=\dfrac{\psi_2''}{\psi_2}$
или
$\psi_1''\psi_2-\psi_1\psi_2'' = 0 (\text{ в виду финитности } \psi_{1,2}(x\to\infty)\to 0) \Rightarrow \dfrac{d}{dx}(\psi_1'\psi_2-\psi_1\psi_2') = 0$
Отсюда следует, что  $\psi_1''\psi_2-\psi_1\psi_2'' = const$. Далее, $const = 0$ из-за поведения $\psi_n(x)$ на бесконечности. В итоге, $\psi_1 = C\psi_2$, где $C-$фазовый множитель.

В одномерной задаче дискретные уровни **четного гамильтониана,** $\hat H(-x) = \hat H(x)$ **имеют определенную четность**, т.е. либо $\psi_n(-x)=+\psi(x)$, либо $\psi_n(-x)=-\psi_n(x)$. Т.е. для такого гамильтониана функции $\psi_n(x)$ и $\psi_n(-x)$ являются решениями, отвечающими одному и тому же значению $E_n$

**Вырождение** — явление, при котором некоторая физическая величина (например. энергия, импульс и т. д.), характеризующая квантовую физическую систему, принимает одно и то же значение для разных состояний квантовой физической системы. Кратностью вырождения называется число различных состояний квантовой физической системы, имеющих одно и то же значение физической величины.

###Билет 3
####Условия сшивки
Сшивка: (условия непрерывности)
1)$\psi(a-\varepsilon)=\psi(a+\varepsilon)$
2)$\dfrac{d\psi}{dx}(a-\varepsilon) = \dfrac{d\psi}{dx}(a+\varepsilon)$
Доказательство(2) $\int\limits_{a-\varepsilon}^{a+\varepsilon}[\dfrac{d^2\psi}{dx^2}+\dfrac{2m}{\hbar^2}(E-U(x))\psi]dx = 0$
$\psi(a-\varepsilon)-\psi(a+\varepsilon)+\dfrac{2mE}{\hbar^2}\cancel{\int\limits_{a-\varepsilon}^{a+\varepsilon}\psi dx} -\dfrac{2mE}{\hbar^2}\cancel{\int\limits_{a-\varepsilon}^{a+\varepsilon}U(x)\psi dx}$
####Прямоугольная яма
Прямоугольная потенциальная яма глубиною $V$ и шириною $2a$
$U(x) = \begin{cases} -V & \text{ при } |x| < a\\
0  & \text{ при } |x| > a
\end{cases}$
$\hat H\psi  = E\psi$
$(\dfrac{p^2_x}{2m}+U(x)) \psi  = E\psi$
$\hat p = -i \hbar \dfrac{d}{dx}$
$(-\dfrac{\hbar^2}{2m}\dfrac{d^2}{dx^2}+U(x)) \psi  = E\psi$
$\dfrac{d^2\psi}{dx^2}+\dfrac{2m}{\hbar^2}(E-U(x))\psi=0$ - стационарное УШ
$\dfrac{p^2}{2m}+U = E$ - классическая механика
$p^2_{classic} = 2m(E-U)$
$\psi'' +\dfrac{p^2_{classic}}{\hbar^2}\psi = 0$
Обозначим $\dfrac{p^2_{classic}}{\hbar^2} = k^2$
Связанным состояниям отвечает энергия $E<0$.
$E<0$ - финитное движение (частица в яме)
$-a \le x \le a$
$\dfrac{d^2\psi}{dx^2}+\dfrac{2m}{\hbar^2}(E+V))\psi=0$
Если $|x| > a \Rightarrow V = 0$
$\dfrac{d^2\psi}{dx^2}+\dfrac{2m}{\hbar^2}E\psi=0$
Введем обозначение $\kappa = \dfrac{1}{\hbar}\sqrt{2m(E+V)}$, тогда
$\dfrac{d^2\psi}{dx^2}+\kappa^2 \psi=0$ (при $|x| > a$)
Имеет следующие решения:
$\psi = A\cos{\kappa x} +B\sin{\kappa x}$
Обозначим $\varkappa = \dfrac{1}{\hbar}\sqrt{2m|E|}$
$\dfrac{d^2\psi}{dx^2}-\varkappa^2\psi=0$ (при $|x| < a$)
Имеет следующие решения:
$\psi = Ce^{-\varkappa x}+De^{\varkappa x}$
Воспользуемся гран условием $\psi(\pm \infty)\equiv 0 \Rightarrow \psi(x) - $ четная функция
**Четные волновые функции**
$\psi(x) = \begin{cases} A\cos{\kappa x} & |x|>a\\
Ce^{-\varkappa x} & x>a\\
Ce^{\varkappa x} & x< -a
\end{cases}$
Сшивка: (условия непрерывности)
1)$\psi(a-\varepsilon)=\psi(a+\varepsilon)$
2)$\dfrac{d\psi}{dx}(a-\varepsilon) = \dfrac{d\psi}{dx}(a+\varepsilon)$
Получим:
$\begin{cases}A\cos{\kappa a} = Ce^{-\varkappa a}\\
A\sin{\kappa a} = Ce^{\varkappa a}\end{cases}$
Из непрерывности $\psi'(x)/\psi(x)$ в точке $x=a$ получаем уравнение
$\kappa\tg{\kappa a} = \varkappa$,
дающее дискретный ряд значений $k_n$ или $E_n$ (энергия квантуется). Найдем их.
Замена: $y = \kappa a$
$\tg{y} = \dfrac{\varkappa a}{y}$
$\varkappa^2 = -\dfrac{1}{\hbar^2}2mE$
$\kappa^2 = \dfrac{1}{\hbar^2}2m(E+V) = \dfrac{2mE}{\hbar^2}+\dfrac{2mV}{\hbar^2}$
$\kappa^2 + \varkappa^2 = \dfrac{2mV}{\hbar^2}$
$\tg y = \dfrac{\varkappa}{\kappa}=\dfrac{\sqrt{\dfrac{2mV}{\hbar^2}-\kappa^2}}{\kappa}= \sqrt{\dfrac{2mV}{\kappa^2\hbar^2}-1}= \sqrt{\dfrac{2mVa^2}{a^2\kappa^2\hbar^2}-1}= \sqrt{\dfrac{2mVa^2}{y^2\hbar^2}-1}$
Замена: $\gamma = \sqrt{\dfrac{\hbar^2}{2mVa^2}}$
Теперь $\tg{y} = \sqrt{\dfrac{1}{\gamma^2y^2}-1}$
Поменяем буковку $y\rightarrow x$
Имеем транцендентное уравнение $\tg{x} = \sqrt{\dfrac{1}{\gamma^2x^2}-1}$
$1+\tg^2{x} = \dfrac{1}{\cos^2x}$
$\begin{cases} \cos x = \pm \varkappa x\\
\tg x \ge 0
\end{cases}$
при $\gamma \ll 1$ (глубокая яма), т.е. $V \gg \dfrac{\hbar^2}{2ma^2}$
$\gamma^2 = \dfrac{\hbar^2}{2ma^2V}$
$x_n = \frac{\pi}{2}+\pi n, n \in \mathbb Z$
$x_n = \frac{\pi}{2}(2n+1)$

$\kappa = \dfrac{x}{a}$
$E=-V+\dfrac{\hbar^2\kappa^2}{2m}$
$E_n=-V+\dfrac{\hbar^2\pi^2N^2}{8ma^2}, N = 1, 3, 5, 7...$
при  $\gamma \to \infty-$ мелкая яма (у мелкой ямы уровень есть всегда)
$\cos{x} = \gamma x$
$x = \frac{1}{\gamma}\cos x$
Замена $\varepsilon = \frac{1}{\gamma}$
$x = \varepsilon\cos x$
$x = c_1\varepsilon +c_2\varepsilon^2+c_3\varepsilon^3+...$
$\cos x = 1 - \frac{x^2}{2}$
$x = \gamma - \dfrac{\gamma x^2}{2}$
$c_1 = 1$
$\gamma - \dfrac{\gamma x^2}{2} = c_1\varepsilon +c_2\varepsilon^2+c_3\varepsilon^3$
$c_1\varepsilon +c_2\varepsilon^2+c_3\varepsilon^3 = \varepsilon(1-\dfrac{c_2^2\varepsilon^2+2c_1c_2\varepsilon+c_2^2\varepsilon^2}{2})$
$c_1\varepsilon +c_2\varepsilon^2+c_3\varepsilon^3 = \varepsilon - \frac{1}{2}\varepsilon^3c_1^2$
$c_1 = 1, c_2 = 0, c_3 = -\frac{1}{2}$
$x = \varepsilon - \dfrac{\varepsilon^3}{2}$
$x = \gamma - \dfrac{\gamma^3}{2}$
$E = -v + \dfrac{\hbar^2x^2}{2ma^2}$
$x^2 = \dfrac{2ma^2}{\hbar^2}-\dfrac{4m^2v^2a^4}{\hbar^4}$
$E = -V + \dfrac{\hbar^2}{2ma^2}\dfrac{2mVa^2}{\hbar^2} = -V +V = 0-$ если брать только $x^2 = \frac{1}{\gamma^2}$ (грубая оценка)
$E = -V + \dfrac{\hbar^2}{2ma^2}(\dfrac{2ma^2V}{\hbar^2}-\dfrac{4m^2v^2a^4}{\hbar^4}) = -\cancel V + \cancel V - \dfrac{2ma^2V^2}{\hbar^2} \ll V$

**Нечетные волновые функции**
$\psi(x) = \begin{cases} A\sin{\kappa x} & |x|\le a\\
Ce^{-\varkappa x} & x\ge a\\
Ce^{\varkappa x} & x \le -a
\end{cases}$

$E = -V + \dfrac{\hbar^2\kappa^2}{2m}$
$E = - \dfrac{\hbar^2\varkappa^2}{2m}$
$\psi'' +\dfrac{2m}{\hbar^2}(E-U(x))\psi=0$
Сшивка:
1)$A\sin{\kappa a} = Be^{-\varkappa a}$
2)$(A\sin{\kappa a})' = (Be^{-\varkappa a})' \Rightarrow \kappa A\cos{\kappa a} = -\varkappa e^{-\varkappa a}$
$\ctg{\kappa a} = -\dfrac{\varkappa}{\kappa}$
$y = \kappa a, \kappa = \frac{\pi }{2a}$
$\ctg{y} = -\sqrt{\dfrac{\pi}{\gamma^2y^2}-1}$
$\ctg^2y+1 = \dfrac{1}{\sin^2y}$
$\sin y = \pm \gamma y$
$y = \frac{\pi}{2}\Rightarrow 1= \gamma \frac{\pi}{2} \Rightarrow \gamma = \dfrac{2}{\pi}$
$\gamma^2 = \dfrac{\hbar^2}{2ma^2}$

$V=\dfrac{\pi^2\hbar^2}{8ma^2}$
при $\gamma \ll 1$, т.е. $V \gg \dfrac{\hbar^2}{2ma^2}$
$y = \pi n, n \in \mathbb Z$
$E = -V+ \dfrac{\hbar^2\pi^2 n^2}{2ma^2}$
####Дельта яма
В яме с глубиной  $V \ll \dfrac{\hbar^2}{ma^2}$ существует только 1 четный уровень и не существует нечетных. Такую яму можно заменить потенциалом $U = -G\delta(x)$
$\psi'' +\dfrac{2m}{\hbar^2}(E+G\delta(x))\psi=0$
при $x\ne 0$
$\psi'' + \dfrac{2mE}{\hbar^2}\psi=0$
$\varkappa^2 = \dfrac{2m|E|}{\hbar^2}$
$\psi''-\varkappa^2\psi=0$
Решение:
$\psi_1=  Ae^{-\varkappa x}, \qquad x>0$
$\psi_2=  Be^{\varkappa x}, \qquad \ \ x<0$
$\Rightarrow \psi = Ae^{-\varkappa|x|}$
Условия сшивки:
$\psi(0)= \psi(-0)\Rightarrow A=B \Rightarrow \int\limits_{-\infty}^{\infty}A^2e^{-2\varkappa|x|}dx = 1\Rightarrow A = \sqrt{\varkappa}$
Условие на скачок. Проинтегрируем УШ в окрестности нуля.
$\int\limits_{-\varepsilon}^{\varepsilon}[\dfrac{d^2\psi}{dx^2} +\dfrac{2m}{\hbar^2}(E+G\delta(x))\psi]dx = 0$
$\psi'(\varepsilon)-\psi'(-\varepsilon)+\cancel{\dfrac{2mE}{\hbar^2}2\varepsilon}+\dfrac{2mE}{\hbar^2}G\int\limits_{-\varepsilon}^{\varepsilon}\psi(x)\delta(x)dx,  \varepsilon\to 0$
$\psi'(\varepsilon)-\psi'(-\varepsilon)+\dfrac{2mG}{\hbar^2}\psi(0) = 0$
Разбиваем формулу $\psi = Ae^{-\varkappa|x|}$ на две:
$x > 0:$
$\psi' = -\varkappa Ae^{-\varkappa x}$
$x < 0:$
$\psi' = -\varkappa Ae^{\varkappa x}$

$-2\varkappa A +\dfrac{2mgA}{\hbar^2} = 0$
$\varkappa = \dfrac{mG}{\hbar^2}$
$\varkappa^2 = \dfrac{2mE}{\hbar^2}$
$E = -\dfrac{\varkappa^2\hbar^2}{2m}=-\dfrac{mG^2}{2\hbar^2}$
$G= 2aV= - \int\limits_{-\infty}^{\infty}U(x)dx$
