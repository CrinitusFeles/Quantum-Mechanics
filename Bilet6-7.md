###Билет 6
####Свойства коммутирующих операторов
Введем коммутатор
$\hat A\hat B \psi, \quad \hat B\hat A\psi \qquad \hat A^{\dagger} = \hat A, \quad \hat B^{\dagger} = \hat B$
Пусть $\begin{cases}
\hat A = \hat p\\
\hat B = \hat x
\end{cases}$
$\begin{cases}
\hat p\hat x \psi(x) = -i\hbar\dfrac{d}{dx}x\psi(x) = -i\hbar\psi - i\hbar x \dfrac{d\psi}{dx}\\
\hat x\hat p \psi(x) = x(-i\hbar\dfrac{d}{dx})\psi = -i\hbar x \dfrac{d\psi}{dx}
\end{cases}$

$[\hat p \hat x -\hat x\hat p]\psi(x) = [\hat p,\hat x]\psi = -i\hbar\psi(x), \quad \forall\psi(x)$
Итак, $[\hat p, \hat x] = -i\hbar, \quad [\hat x, \hat p] = i\hbar \ - $коммутатор
**Свойства:**
$$[\hat A+\hat B, \hat C] = [\hat A,\hat C] + [\hat B, \hat C]$$

$$[\hat A, \hat B] = -[\hat B, \hat A]$$

$$[\hat A, \hat B\hat C] = \hat B[\hat A,\hat C]+[\hat A,\hat B]\hat C$$
####Измеримость величин
Физические величины $\hat F$ и $\hat G$ называются *измеримыми совместно*, если существуют такие состояния, в каждом из которых будет измерима как величина $F$, так и $G$. Математически это выражается в наличии у операторов $\hat F$ и $\hat G$ *общих* собственных функций. Существование общих собственных функций проверяется с помощью следующего критерия:
*необходимым и достаточным условием существования у линейных 4 операторов общих собственных функций является коммутация данных операторов.*

У операторов неизмеримых совместно величин, естественно, общих собственных функций нет. При совместном измерении таких величин в *произвольном* состоянии *всегда наблюдается разброс наблюдаемых значений*. Величина этого разброса, характеризуемая среднеквадратичными отклонениями, удовлетворяет неравенству
$$\langle(\Delta F)^2\rangle\langle(\Delta G)^2\rangle\ge\dfrac{1}{4}\langle B\rangle^2$$

называемому *соотношением неопределенностей Гейзенберга*. Здесь $\hat B$ — самосопряженный оператор, определяемый из соотношения:
$$[\hat F,\hat G] = i\hat B$$

Все усреднения в (3.21) производятся в одном и том же состоянии.
Теперь можно легко вывести соотношения неопределенностей для координаты и импульса, нужно лишь воспользоваться равенством $[x,p_x]=i\hbar$ и заменить $F\to x, g\to p_x, B\to\hbar$ в итоге получим:
$$\langle(\Delta x)^2\rangle\langle(\Delta p_x)^2\rangle\ge\dfrac{1}{4}\hbar^2$$

Если величины $A$ и $B$ одновременно измеримы, то существует полная система волновых функций $\psi_n$, таких, что $\psi_n -$ одновременно собственная функция и $\hat A,$ и $\hat B$. Но тогда
$$\hat A \hat B \psi = \hat A \hat B \sum\limits_n c_n\psi_n = \sum\limits_n c_n ab \psi_n = \sum\limits_n c_n \hat B \hat A \psi_n = \hat B\hat A\psi,$$

то есть
$$[\hat A\hat B]\equiv\hat A\hat B - \hat B\hat A = 0$$

И обратно, если $\hat A\hat B = 0$, то $\hat A$ и $\hat B$ могут иметь общую систему собственных функций. Пусть $\psi_a - $собственная функция $\hat A$:
$$\hat A\psi_a = a\psi_a,$$

тогда
$$\hat B\hat A\psi_a = a\hat B\psi_a=\hat A \hat B\psi_a,$$

то есть $\hat B\psi_a -$ тоже собственная функция $\hat A$ с собственным значением $a$. Если спектр невырожден, отсюда следует, что $\hat B\psi_a$ с точностью до множителя совпадает с $\psi_a$, то есть $\hat B\psi_a = b\psi_a$, так что $\psi_a$, действительно, является собственной функцией оператора $\hat B$ (с собственным значением $b$). В случае вырожденного спектра можно выбрать такие линейные комбинации $\sum_i c_i\psi_{ai}$ собственных функций оператора $\hat A$, которые будут одновременно собственными функциями $\hat B$.
####Вырожденность спектра
Пусть есть $\begin{cases}
[\hat H, \hat A] = [\hat H, \hat B] = 0 \\
\ [\hat A, \hat B] \ne 0
\end{cases}$
$\hat H\psi_n=E_n\psi_n$
$A\psi_n=a_n\psi_n$
$\hat B\psi_n - ?$
Подействуем:
$\hat H(\hat B\psi_n)=E_n(B\psi_n)\qquad B\psi_n\ne b_n\psi_n$
Можно выбрать такие коммутации $\sum_i c_i\psi_{ni}$ собственных функций оператора $\hat A$, которые будут одновременно собственными функциями $\hat B$.
###Билет 7
####Вывод соотношения неопределённостей для координаты и импульса
Определим дисперсию
$$\Delta A = \sqrt{\langle(A-\langle A\rangle)^2\rangle}.$$

Пусть эрмитовы операторы $\hat A$ и $\hat B$ не коммутируют, $[\hat A, \hat B] = i\hbar\hat C$ ($i-$нужна , т.е. $\hat A,\hat B,\hat C$ эрмитовы и при сопряжении ничего меняться не должно) и для простоты $\langle n |\hat A|n\rangle = \langle n |\hat B|n\rangle = 0.$
Определим
$$\Delta A \Delta B= \sqrt{\langle(A-\langle A\rangle)^2\rangle}\sqrt{\langle(B-\langle B\rangle)^2\rangle}\ge\frac{\hbar}{2}\sqrt{\langle C \rangle^2}.$$

$$\Delta \hat x = \hat x - \langle x \rangle \qquad \Delta \hat p = \hat p - \langle p \rangle$$

Рассмотрим интеграл вида:
$\int\psi^* (\underbrace{\alpha\Delta \hat x-i\Delta\hat p}_{\hat l^+})(\underbrace{\alpha\Delta\hat x + i\Delta\hat p}_{\hat l})\psi(x)dx = \int(L\psi^* )(L\psi)dx = \int|L\psi|^2dx\ge 0 \quad =0, \text{ когда } \hat L\psi = 0$

Воспользуемся положительной определенностью
$\int|L\psi|^2dx = \langle \alpha^2(\Delta x)^2\rangle-\langle i \Delta\hat p\ \alpha\Delta\hat x\rangle + \langle\alpha\Delta\hat x\ i\Delta\hat p \rangle +\langle\Delta\hat p \rangle^2=$
$=\langle\alpha^2(\Delta\hat x)^2\rangle+i\alpha\langle[\Delta\hat x,\Delta\hat p]\rangle+\langle(\Delta\hat p)^2\rangle =
\begin{cases}[\hat A,\hat B] = i\hbar \hat C\\ \lbrack\Delta\hat x, \Delta\hat p] =[\hat x,\hat p] = i\hbar \end{cases}$
$=\alpha^2\langle(\Delta\hat x)^2\rangle-\alpha\hbar +\langle(\Delta\hat p)^2\rangle\ge0$

Для выполнения неравенства, решаем квадратное уравнение:
$\alpha_{1,2} =\dfrac{\hbar \pm\sqrt{\hbar^2-4\langle(\Delta\hat x)^2\rangle\langle(\Delta\hat p)^2\rangle}}{2\langle(\Delta\hat x)^2\rangle}=\dfrac{\hbar}{2\langle(\Delta\hat x)^2\rangle}\pm\sqrt{\underbrace{\dfrac{\hbar^2}{4\langle(\Delta\hat x)^2)\rangle^2}-\dfrac{\langle(\Delta\hat p)^2\rangle}{\langle(\Delta\hat x)^2\rangle}}_{\le0}}$
Максимум: $\alpha = \dfrac{\hbar}{2\langle(\Delta\hat x)^2\rangle}$

Подставим $\alpha = \dfrac{\hbar}{2\langle(\Delta\hat x)^2\rangle}$ в неравенство:
$$\dfrac{\hbar^2}{4\langle(\Delta\hat x)^2\rangle}-\dfrac{\hbar^2}{2\langle(\Delta\hat x)^2\rangle}+\langle(\Delta\hat p)^2\rangle\ge0$$

$$\langle\Delta\hat x^2\rangle\langle\Delta\hat p^2\rangle \ge \dfrac{\hbar^2}{4}\Rightarrow \sqrt{\langle\Delta\hat x^2\rangle}\sqrt{\langle\Delta\hat x^2\rangle}\ge \dfrac{\hbar}{2}$$

Это и есть соотношения неопределённостей для координаты и импульса.

Что произойдет, если будет выполняться условие $L\psi=0$?, т.е.
$$(\alpha\langle\Delta\hat x\rangle+i\langle\Delta\hat p\rangle)\psi = 0$$

$$(\alpha x +\hbar \dfrac{d}{dx})\psi = (\alpha\langle x\rangle + i\langle p\rangle)\psi$$

$\psi = \tilde \psi e^{\frac{i\langle p\rangle x}{\hbar}}\Rightarrow\Bigl (\alpha(x - \langle x\rangle)+\dfrac{\hbar d}{d(x - \langle x\rangle)}\Bigl )\tilde \psi $
$\tilde\psi' = \dfrac{-\alpha}{\hbar}(x - \langle x\rangle)\tilde\psi\Rightarrow\dfrac{d\tilde\psi}{\tilde\psi}=\dfrac{-alpha}{\hbar}(x - \langle x\rangle)d(x - \langle x\rangle)$
$\psi(x) = Ce^{-\frac{(x - \langle x\rangle)^2}{4\langle\Delta x^2\rangle}+i\frac{\langle p\rangle x}{\hbar}}=\dfrac{1}{\sqrt{\sqrt{\pi\langle\Delta x^2\rangle}}}e^{-\frac{(x - \langle x\rangle)^2}{4\langle\Delta x^2\rangle}+i\frac{\langle p\rangle x}{\hbar}}$
$\int|\psi(x)|^2dx =1\Rightarrow C=\dfrac{1}{\sqrt{\sqrt{\pi\langle\Delta x^2\rangle}}} - $волновая функция, минимизирующая соотношения неопределённостей для $\hat x$ и $\hat p$.

####Использование соотношений неопределённостей для оценки энергии основного состояния дискретного спектра
$$\Delta x\Delta p \ge \dfrac{\hbar}{2}$$

Атом водорода: $E = \dfrac{p^2}{2m}-\dfrac{e^2}{r}\qquad \Delta x = \sqrt{\sqrt{\langle(x -\langle x \rangle)^2\rangle}} \quad\Delta x = \sqrt{\sqrt{\langle(p -\langle p \rangle)^2\rangle}}$
$\langle x \rangle = 0, \quad \langle p\rangle =0 -$ равновероятно
$$\langle p\rangle = \Delta p\quad \langle x \rangle = \Delta x$$

$$\Delta p\Delta x \sim \hbar$$

$\langle E\rangle = \dfrac{(\Delta p)^2}{2m}-\dfrac{e^2}{r}=\Biggr[\Delta p \sim \dfrac{\hbar}{\Delta x}\Biggr] = \dfrac{\hbar^2}{2m(\Delta x)^2}-\dfrac{e^2}{\Delta x}$
$(\langle E\rangle)'=0=-\dfrac{\hbar^2}{m(\Delta x)^3}+\dfrac{e^2}{(\Delta x)^2}=0 \Rightarrow$
$\Rightarrow \dfrac{\hbar^2}{m}=e^2\Delta x \Rightarrow \Delta x = \dfrac{\hbar^2}{e^2m}\approx 0,5 \overset{\circ}{\mathbf A} -\text{ Боровский радиус}$

$E =\dfrac{\hbar^2e^2m^2}{2m\hbar^4}-\dfrac{e^2e^2m}{\hbar^2}=\dfrac{e^4m}{2\hbar^2}-\dfrac{e^2m}{\hbar^2}=-\dfrac{me^4}{2\hbar^2}=13,6\text{ эВ}$
