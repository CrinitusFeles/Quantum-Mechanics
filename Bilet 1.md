###Билет 1
####Волновая функция
Свойства атомных объектов в квантовой механике описываются с помощью вспомогательной величины - *волновой функции* или *вектора состояния*. Волновая функция, описывающая состояние движения одной частицы, является комплексной однозначной и непрерывной функцией радиуса-вектора $\vec r$ и времени $t$. Волновая функция $\psi(\vec r, t)$ удовлетворяет некоторому дифференциальному уравнению (*уравнение Шредингера*), которое и определяет характер движения частицы.
У волновой функции *нет универсальной размерности*. Ее размерность определяется только элементом интегрирования: $[\psi(r,t)] = [dr]^{-1/2}.$
В качестве волновой функции может выступать не любая математическая функция, а удовлетворяющая стандартным условиям: конечная, однозначная и непрерывная. Первые два условия непосредственно
следуют из ее вероятностной интерпретации
####Вероятностная интерпретация
Сама волновая функция физического смысла не имеет, но физический смысл приписывается квадрату её модуля $ {\displaystyle \left|\Psi (x_{1},x_{2},\ldots ,x_{n},t)\right|^{2}}$, который интерпретируется как плотность вероятности $\omega$  (для дискретных спектров — просто вероятность) обнаружить систему в положении, описываемом координатами ${\displaystyle x_{1}=x_{01},x_{2}=x_{02},\ldots ,x_{n}=x_{0n}}$ в момент времени $t:$

$${\displaystyle \omega ={\dfrac {dP}{dV}}=\left|\Psi (x_{1},x_{2},\ldots ,x_{n},t)\right|^{2}=\Psi ^{\ast }\Psi } .$$

Тогда в заданном квантовом состоянии системы, описываемом волновой функцией ${\displaystyle \Psi (x_{1},x_{2},\ldots ,x_{n},t)} $, можно рассчитать вероятность $P$ того, что частица будет обнаружена в любой области конфигурационного пространства конечного объема $V:$
 $${\displaystyle P={\int {dP}}={\int\limits_{V}{\omega }dV}={\int\limits_{V}{\Psi^{\ast }\Psi }dV}}$$

 ***
 Если мы хотим, чтобы суммарная вероятность всех возможных исходов какого-то измерения была равна единице, то это можно записать в виде нормировочного условия (нормировки) для волновой функции:
 $$\langle\psi|\psi\rangle = 1$$

 Если переменная x пробегает непрерывные значения из области $U$ и дискретные из множества $W$, то
 $$\langle\phi|\psi\rangle = \int\limits_U\phi^* (x)\psi(x)dx+\sum\limits_{k\in W}\phi^* (k)\psi(k)$$

 Если расписать скалярный квадрат через интеграл и сумму согласно формуле выше, то мы получим интеграл от плотности вероятности $\psi^* (x)\psi(x)$ для непрерывного спектра $(x \in U)$ и сумму вероятностей $\psi^* (k)\psi(k)$ для дискретного спектра $(k \in W)$

  $$\langle\psi|\psi\rangle = \int\limits_U\psi^* (x)\psi(x)dx+\sum\limits_{k\in W}\psi^* (k)\psi(k)$$

Здесь *спектр физической величины* — набор значений, которые эта величина может принимать.

Условие $\langle\psi|\psi\rangle = 1$ называется *нормировкой на единицу* (или *условием нормировки на единицу*). Поскольку волновая функция определена с точностью до числового множителя, на единицу может быть отнормирована любая волновая функция с конечным скалярным квадратом:

$$|\psi_{\text{норм.}}\rangle=\dfrac{|\psi\rangle}{\sqrt{\langle\psi|\psi\rangle}}$$

Умножение на фазовый множитель $e^{i\alpha}\ \  (\alpha \in \mathbb R, |e^{i\alpha}| =1)$ не нарушаетнормировку волновой функции.
***
**Нормировка на вероятность**

Таким образом, мы можем считать, что физический смысл скалярного квадрата волновой функции — полная вероятность. Обычно мы нормируем волновую функцию на единицу, но, рассматривая волновую функцию *после измерения*, может быть удобно нормировать волновую функцию на вероятность рассматриваемого исхода.

Если до измерения система находилась в состоянии $|\psi\rangle$, в результате измерения некоторой дискретной величины $k$ система попадает в одно из ортогональных состояний $|\phi_k\rangle$. Причем, мы можем отнормировать эти состояния так, что
$$|\psi\rangle=\sum\limits_k|\phi_k\rangle,$$

$$\langle\phi_k|\phi_{k'}\rangle=p_k\delta_{kk'},$$

$$\langle\phi|\phi\rangle=\sum\limits_{kk'}\langle\phi_k|\phi_{k'}\rangle=\sum\limits_kp_k=1,$$

где $p_k$ — вероятность исхода номер $k$.

Волновые функции $|\phi_k\rangle$ получаются из $|\psi\rangle$ с помощью соответствующего данной измеряемой величины набора проекторов $\hat P_k$:
 $$|\phi_k\rangle=\hat P_k|\psi\rangle,$$

$$\hat P_k\hat P_{k'}=\hat P_k\delta_{kk'},$$

$$\sum\limits_k\hat P_k=\hat 1.$$

Проекторы $\hat P_k$ отображают векторы состояния на одномерное подпространство, если для данного $k$ существует только одно линейно независимое собственное состояние (невырожденное состояние). В общем случае размерность области значений оператора $\hat P_k$ может быть произвольной, в том числе бесконечной.
***
**Амплитуда при измерении и скалярное произведение**

Вероятность $p_k$ некоторого исхода измерения можно записать в следующем виде:
$$\langle\phi_k|\psi\rangle=\langle\phi_k|\sum\limits_{k'}|\phi_{k'}=\sum\limits_{k'}\langle\phi_k|\phi_{k'}\rangle=\sum\limits_{k'}p_k\delta_{kk'}=p_k.$$

Однако при этом начальная волновая функция $\psi$ и конечная — $\phi_k$ нормированы по-разному: одна на единицу, а другая на вероятность.

Если обе волновые функции, начальную $\psi$ и конечную $\phi$, отнормировать на единицу, то скалярное произведение дает амплитуду вероятности того, что система, находившаяся в состоянии $\psi$, будет обнаружена в состоянии $\phi$. Другими словами, мы имеем систему в состоянии $\psi$ и ставим опыт, который должен ответить на вопрос: «А не находится ли система в состоянии $\phi$?» Причем если ответ будет положительным, то система и в самом деле окажется в этом состоянии. Скалярное произведение
$$A_{\phi\psi}=\langle\phi|\psi\rangle$$

задает соответствующую амплитуду вероятности.

Сама вероятность имеет вид
$$p_{\phi\psi}=|\langle\phi|\psi\rangle|^2=\langle\psi|(|\phi\rangle\langle\phi|)|\psi\rangle=\langle\psi|\hat P_{\phi}|\psi\rangle=tr(\hat P_{\psi}\hat P_{\phi}),$$

$$\hat P_{\psi}=|\psi\rangle\langle\psi|,\qquad \hat P_{\phi}=|\phi\rangle\langle\phi|.$$

Оператор $\hat P_{\psi}$ представляет собой проектор на направление $\phi$.
####Среднее значение физический величины
Плотность вероятности найти частицу в точке $x$ — величина $\dfrac{dW}{dx}$ — пропорциональна$|\psi(x,t)|^2$.  Если $ψ(x,t)$ нормирована условием

$$\int|\psi(x,t)|^2dx = 1,$$

 то
 $$\dfrac{dW}{dx} = |\psi(x,t)|^2.$$

Тогда среднее значение $x$ равно
$$\langle x \rangle  = \int x dW = \int x |\psi(x,t)|^2 dx = \int\psi^* (x) x \psi(x)dx.$$

Аналогично, среднее значение любой функции $F(x)$ равно

$$\langle F(X)\rangle = \int \psi^* (x) F(x) \psi(x)dx$$

Если же используется ненормированная волновая функция финитного движения, то
$$\langle F\rangle = \dfrac{\int \psi^* (x) F(x) \psi(x)dx}{\int|\psi(x,t)|^2dx}$$

Среднее значение по своему смыслу должно быть величиной вещественной.

Описанный выше способ измерения физической величины $F$ дает с математической точки зрения последовательность случайных чисел. Характеристикой их разброса относительно среднего значения служит *среднеквадратичное отклонение:*
$$\langle(\Delta F)^2\rangle = \langle(F-\langle F\rangle)^2\rangle$$

Более удобной формулой для вычисления $\langle(\Delta F)^2\rangle$ по сравнению с предыдущей является
$$\langle(\Delta F)^2\rangle = \langle F^2\rangle - \langle F\rangle^2.$$

####Операторы координаты и импульса
В координатном представлении (в базисе собственных функций оператора координаты) базисные функции самого координатного базиса имеют вид, обычный для непрерывного спектра:
$$\phi_{x_0}(x)=\langle\phi_x|\phi_{x_0}\rangle=\delta(x-x_0).$$

В том же координатном представлении базис собственных функций оператора импульса задается волнами де Бройля:
$$\phi_{p_0}(p)=\langle\phi_p|\phi_{p_0}\rangle=\dfrac{1}{\sqrt{2\pi\hbar}}e^{\frac{i}{\hbar}p_0x}.$$

В импульсном представлении (в базисе волн де Бройля)
$$\phi_{p_0}(p)=\langle\phi_p|\phi_{p_0}\rangle=\delta(p-p_0).$$

В том же импульсном представлении базис собственных функций оператора координаты зада¨ется комплексным сопряжением волн де Бройля:

$$\phi_{x_0}(x)=\langle\phi_p|\phi_{x_0}\rangle=\langle\phi_{x_0}|\phi_{p}\rangle^* = \dfrac{1}{\sqrt{2\pi\hbar}}e^{\frac{i}{\hbar}p_0x}.$$

Таким образом, координатное и импульсное представление связаны друг с другом преобразованием Фурье (см. Приложения).

В своем представлении каждый оператор действует умножением на аргумент волновой функции. Операторы импульса в координатном и координаты в импульсном представлении задаются как дифференциальные операторы.

В $x-$пространстве:
$$\hat x \psi(x)= x\psi(x)$$

$$\hat p \psi(x)= -i \hbar \dfrac{d}{dx}\psi(x)$$

В $p-$ пространстве
$$\hat x \psi(p)= i \hbar \dfrac{d}{dx}\psi(p)$$

$$\hat p \psi(p)= p\psi(p)$$

Коммутатор операторов $\hat p$ и $\hat x$ вне зависимости от представления имеет вид: $[\hat x, \hat p_x] = i\hbar$

Докажем это:
$$[\hat x, \hat p_x]\psi=x\hat p_x\psi-\hat p_x x\psi$$

$$x\hat p_x\psi=x(\hat p_x\psi)=-i\hbar\dfrac{\partial\psi}{\partial x};$$

$$\hat p_xx\psi=\hat p_x(x\psi)=-i\hbar\dfrac{\partial}{\partial x}(x\psi)=-i\hbar\psi-i\hbar x\dfrac{\partial \psi}{\partial x}.$$

$$[\hat x, \hat p_x]\psi = i\hbar\psi$$

$$\fbox{[\hat x, \hat p_x] = i\hbar}$$

Именно это уравнение можно считать «настоящим» определением координаты и импульса.

Из операторов $\hat r$ и $\hat p$ строятся все динамические переменные. Например, оператор момента импульса
$$\hat M = \hat r\times\hat p = -i\hbar r \times \nabla.$$

**Пример:** Частица приведена в состояние с волновой функцией
$$\psi(x)=\begin{cases}A\sin{\dfrac{\pi x}{a},} &\text{при } 0\le x\le a;\\
0, & \text{при } x< 0 \text{ или }x> a.
\end{cases}$$

Вычислить нормировочную константу A.
**Решение:**
Частица локализована в конечной области пространства, поэтому в качестве условия нормировки следует взять $\int|\psi(x,t)|^2dx = 1:$
$$1=|A|^2\int\limits_0^a\sin^2{\dfrac{\pi x}{a}}\ dx=\dfrac{1}{2}|A|^2\int\limits_0^a\biggr[1-\sin^2\dfrac{2\pi x}{a}\biggr]dx=\dfrac{a}{2}|A|^2.$$

Интеграл от второго слагаемого обращается в нуль из-за интегрирования гармонической функции по ее периоду. Таким образом, с точностью до фазового множителя $A =\sqrt{\dfrac{2}{a}}$, а нормированная функция
$$\fbox{\psi(x)=\sqrt{\dfrac{2}{a}}\sin{\dfrac{\pi x}{a}}}$$

**Пример:** *Волновой пакет задается функцией
$$\psi(x) = A\ exp\biggr[-\dfrac{x^2}{2x_0^2}+ik_0x\biggr],$$ где $x_0 > 0$ — константа с размерностью длины, определяющая ширину пакета, $k_0$ — константа с размерностью волнового числа. Вычислить нормировочную константу $A$.*
**Решение:**
При возведении $|\psi(x|)$ в квадрат слагаемое $ik_0x$ под знаком экспоненты исчезает и задача сводится к вычислению интеграла
$$\int\limits_{-\infty}^{\infty}exp\biggr[-\dfrac{x^2}{x_0^2}\biggr]dx$$

с помощью замены переменных $\dfrac{x}{x_0}= t$ сводится к интегралу Пуассона, так что $|A|^2=\dfrac{1}{x_)\sqrt{\pi}}$. Окончательный **ответ:**
$$\fbox{\psi(x) = \dfrac{1}{\sqrt{x_0\sqrt{\pi}}}e^{-\frac{x^2}{2x_0^2}}}$$

*А теперь для этого же волнового пакета вычислим $\langle x\rangle,\ \langle(\Delta x)^2\rangle,\ \langle p_x\rangle,\ \langle(\Delta p_x)^2\rangle.$*
**Решение:**
Нормировочная константа уже вычислена, так что нормированная волновая функция имеет вид
$$\psi(x) = \dfrac{1}{\sqrt{x_0\sqrt{\pi}}}e^{-\frac{x^2}{2x_0^2}+ik_0x}$$

а средние значения вычисляются по формуле $\langle F(X)\rangle = \int \psi^* (x) F(x) \psi(x)dx$

Для координаты
$$\langle x\rangle = \dfrac{1}{x_0\sqrt\pi}\int\limits_{-\infty}^{\infty}exp\biggr[-\dfrac{x^2}{x_0^2}\biggr]dx = 0$$

вследствие нечетности подынтегральной функции. Обратите внимание на исчезновение множителя $e^{ik_0x}$ при возведении его модуля в квадрат!

Для среднеквадратичного отклонения координаты
$$\langle(\Delta x)^2\rangle = \langle x^2\rangle - \langle x\rangle^2=\langle x^2\rangle=\dfrac{1}{x_0\sqrt\pi}\int\limits_{-\infty}^{\infty}exp\biggr[-\dfrac{x^2}{x_0^2}\biggr]dx=$$

$$=\biggr[x=x_0\varepsilon\biggr]=\dfrac{x_0^2}{\sqrt\pi}\int\limits_{-\infty}^{\infty}\varepsilon^2e^{-\varepsilon^2}d\varepsilon = \dfrac{x_0^2}{2}$$

Оператор импульса - дифференциальный. Поэтому
$$\langle p_x\rangle = \int\limits_{-\infty}^{\infty}\psi^* (x)p_x\psi(x)dx=-i\hbar\int\limits_{-\infty}^{\infty}\psi^* (x)\dfrac{\partial\psi(x)}{\partial x}dx =$$

$$=-\dfrac{i\hbar}{x_0\sqrt\pi}\int\limits_{-\infty}^{\infty}(-\dfrac{x}{x_0^2}+ik_0)exp\biggr[-\dfrac{x^2}{x_0^2}\biggr]dx = \hbar k_0;$$

$$\langle p_x^2\rangle=\int\limits_{-\infty}^{\infty}\psi^* (x)p_x^2\psi(x)dx=-\hbar^2\int\limits_{-\infty}^{\infty}\psi^* (x)\dfrac{\partial^2\psi(x)}{\partial x^2}dx=$$

$$-\hbar^2\underbrace{\psi^* (x)=\dfrac{\partial\psi(x)}{\partial x}\Bigg |_ {-\infty}^{\infty}}_{0}+\hbar^2\int\limits_{-\infty}^{\infty}\bigg| \dfrac{\partial\psi(x)}{\partial x}\bigg |^2dx=$$

$$=\dfrac{\hbar^2}{x_0\sqrt\pi}\int\limits_{-\infty}^{\infty}(\dfrac{x^2}{x_0^4}+k_0^2)exp\biggr[-\dfrac{x^2}{x_0^2}\biggr]dx = \dfrac{\hbar^2}{2x_0^2}+\hbar^2 k_0^2;$$

$$\langle(\Delta p_x)^2\rangle=\langle p_x^2\rangle - \langle p_x\rangle^2=\dfrac{\hbar^2}{2x_0^2}$$
****
####Приложения
#####Преобразование Фурье
Рассмотрим пространство $L_2(\mathbb R)$ (квадратично интегриремых функций) и базис, состоящий из волн де Бройля (состояний с определенным импульсом $\hbar k$):
$$\xi_k(x)=\dfrac{1}{\sqrt{2\pi}}e^{ikx}=\langle\phi_x|\xi_k\rangle,\quad k\in\mathbb R.$$

Здесь $\phi_{x_0}(x)=\delta(x-x_0)$ — волновые функции исходного базиса (состояния с определенным значением координаты x0)

Переход к новому базису соответствует преобразованию Фурье. Этот базис является ортонормированным, т.е.
$$\langle\xi_k|\xi_l\rangle=\delta(k-l).$$

Хотя матричный элемент $\langle\xi_k|\xi_l\rangle$ является обобщенной функцией, при $k \ne l$ она имеет хорошо определенное (нулевое) значение, однако соответствующий интеграл
$$\langle\xi_k|\xi_l\rangle=\dfrac{1}{2\pi}\int\limits_{-\infty}^{+\infty}e^{i(l-k)x}dx$$

расходится. При стремлении к бесконечности пределов интегрирования

$$\int\limits_{-R}^{+R}e^{i(l-k)x}dx=\dfrac{2\sin((l-k)R)}{l-k}, \quad R\to+\infty$$

значение интеграла колеблется, но не стремится к какому-либо пределу. Мы можем домножить подынтегральное выражение на какой-либо регуляризующий фактор, например $e^{-\alpha |x|}$, после чего перейти к пределу $\alpha\to 0$, но смысл формулы $\langle\xi_k|\xi_l\rangle=\delta(k-l)$ не в этом, а в том, что скалярное произведение для функций и их преобразования Фурье записывается одинаково:
$$\langle\phi|\psi\rangle=\int\limits_{-\infty}^{+\infty}\phi^* (x)\psi(x)dx=\int\limits_{-\infty}^{+\infty}\phi^* (k)\psi(k)dk,$$

$$\phi^* (k) = \langle\phi|\xi_k\rangle = \int\limits_{-\infty}^{+\infty}\phi^* (x)\dfrac{e^{ikx}}{\sqrt{2\pi}}dx,\quad\psi(k)=\langle\xi_k|\psi\rangle=\int\limits_{-\infty}^{+\infty}\dfrac{e^{-ikx}}{\sqrt{2\pi}}\psi(x)dx.$$

Поскольку $|\psi\rangle = \int\limits_{-\infty}^{+\infty}\psi(x)|\phi_x\rangle dx=\int\limits_{-\infty}^{+\infty}\psi(k)|\xi_xdk$ мы можем удобно записать друг через друга $\psi(k)=\langle\xi_k|\psi\rangle$ и $\psi(x)=\langle\phi_x|\psi\rangle,$ используя ядро $\langle\xi_k|\phi_x\rangle=\langle\phi_x|\xi_k\rangle^* :$

$$\psi(k)=\int\limits_{-\infty}^{+\infty}\langle\xi_k|\phi_x\rangle\psi(x)dx,\quad\psi(x)=\int\limits_{-\infty}^{+\infty}\dfrac{e^{ikx}}{\sqrt{2\pi}}\psi(k)dk=\int\limits_{-\infty}^{+\infty}\langle\phi_x|\xi_k\rangle\psi(k)dk$$

Если величина $x$ безразмерна, то $k$ тоже безразмерна и мы можем рассматривать преобразование Фурье по своему выбору как замену базиса, либо как унитарное преобразование. Если же $x$ и $k $размерны, то мы можем рассматривать преобразование Фурье как замену базиса, но не можем рассматривать их как унитарное преобразование, впрочем, мы всегда можем обезразмерить переменные, разделив $x$ и умножив $k$ на некоторую константу $x_0$ с размерностью $x$.

Часто в физике в качестве аргумента преобразования Фурье выбирается не волновое число $k$, а импульс $p = \hbar k$. В этом случае нормированные волновые функции нового базиса должны быть поделены на $\sqrt\hbar$:
$$\xi_p(x)=\dfrac{1}{\sqrt{2\pi\hbar}}e^{\frac{i}{\hbar}px},\qquad p\in \mathbb R.$$