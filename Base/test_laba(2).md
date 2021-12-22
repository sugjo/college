---
tags:
- тестирование
- лаба
---
<h5 align="center">Лабораторная работа № 2</h5>

<h5 align="center">Cравнительный анализ технологий разработки интеллектуальных систем</h5>

**Цель работы:** 
провести сравнительный анализ средств разработки ИС анализа иерархий Т. Саати.

<h5 align="center">Ход работы:</h5>

<h4 align="center">Задание:</h4>

Необходимо провести сравнительный анализ выбора средств разработки ИС для дальнейшего практического использования.
Для решения задачи необходимо
- выполнить сбор информации по наиболее распространенным МАС,
- определить достоинства и недостатки средств разработки
- выполнить сравнительный анализ при помощи метода иерархий Т.Саати
- построение иерархии;
- построение матрицы парных сравнений;
- проверка согласованности матриц;
- синтез приоритетов на иерархии.

На основе МАИ нужно выполнить сравнение альтернатив из рис.1 по следующим критериям:
- наличие лицензия Freeили LGPL;
- поддержка языка программирования Java;
- возможность создание приложение под Android;
- наличие достаточного описания в литературе
- наличие примеров.

*Табл.*

| №   | Наименование | Лицензия                 | Поддержка языка программирования | Создание приложение под Android | Наличие документации | Примеры |
| --- | ------------ | ------------------------ | -------------------------------- | ------------------------------- | -------------------- | ------- |
| 1   | JADE         | LGPL V2                  | Java                             | Да                              | Англ. док.           | Есть    |
| 2   | MadKIT       | LGPL и GPL               | JVM(Java 2)                      | Нет информации                  | Англ. док.           | Есть    |
| 3   | AgentBuilder | Закрытая                 | Java; C; C++                     | Нет информации                  | Англ. док            | Есть    |
| 4   | Cougaar      | COSL                     | Java                             | Нет информации                  | Англ. док            | Нет     |
| 5   | NetLogo      | Free, nt open source     | NetLogo                          | Нет информации                  | Англ. док            | Есть    |
| 6   | VisualBots   | Неизвестно               | Visual Basic                     | Нет информации                  | Англ. док            | Есть    |
| 7   | MASON        | Free для учеб. заведений | Java                             | Нет                             | Англ. док            | Есть    | 

![](../Files/Pasted%20image%2020211222203039.png)

Согласованность суждения оценивается индексом однородности (индексом согласованности) или отношением однородности (отношением согласованности) в соответствии со следующими формулами:

![](../Files/Pasted%20image%2020211222211530.png)
![](../Files/Pasted%20image%2020211222211534.png)

M(uo) - среднее значение индекса однородности случайным образом составленной матрицы парных сравнений, которое основано на экспериментальных данных. Значение есть табличная величина, входным параметром выступает размерность матрицы (таблица).

<table class="table table-bordered table-center"><tbody><tr><td align="center">n</td><td align="center">1</td><td align="center">2</td><td align="center">3</td><td align="center">4</td><td align="center">5</td><td align="center">6</td><td align="center">7</td><td align="center">8</td><td align="center">9</td><td align="center">10</td><td align="center">11</td></tr><tr><td align="center">M(ио)</td><td align="center">0</td><td align="center">0</td><td align="center">0.58</td><td align="center">0.9</td><td align="center">1.12</td><td align="center">1.24</td><td align="center">1.32</td><td align="center">1.41</td><td align="center">1.45</td><td align="center">1.49</td><td align="center">1.51</td></tr></tbody></table>

В качестве допустимого используется значение OO ≤ 0.1 . Если для матрицы парных сравнений OO > 0.1, то это свидетельствует о существенном нарушении логики суждений, допущенном экспертом при заполнении матрицы, поэтому эксперту предлагается пересмотреть данные, использованные для построения матрицы, чтобы улучшить однородность.  
Алгоритм иерархического синтеза.  
1. Определим векторы приоритетов Wi относительно последнего уровня иерархии. Для этого строим матрицы парных сравнений [Ei] и вычисляем для каждой из матриц максимальные собственные значения (для оценки однородности суждений) и главные собственные вектора (приоритеты).  
2. Аналогичным образом обрабатываем матрицы парных сравнений для вышележащих уровней. Данные матрицы построены для того, чтобы определить предпочтительность элементов определенного иерархического уровня относительно элементов вышележащего.

<table class="table table-bordered table-center"><tbody><tr><td align="center"> </td><td align="center">наличие лицензии</td><td align="center">поддержка языка Java</td><td align="center">оздание приложение под Android</td><td align="center">Наличие документации</td><td align="center">Примеры</td></tr><tr><td align="center">наличие лицензии</td><td align="center">1</td><td align="center">3</td><td align="center">8</td><td align="center">4</td><td align="center">3</td></tr><tr><td align="center">поддержка языка Java</td><td align="center"><sup>1</sup>/<sub>3</sub></td><td align="center">1</td><td align="center">6</td><td align="center">6</td><td align="center">4</td></tr><tr><td align="center">оздание приложение под Android</td><td align="center"><sup>1</sup>/<sub>8</sub></td><td align="center"><sup>1</sup>/<sub>6</sub></td><td align="center">1</td><td align="center">3</td><td align="center">5</td></tr><tr><td align="center">Наличие документации</td><td align="center"><sup>1</sup>/<sub>4</sub></td><td align="center"><sup>1</sup>/<sub>6</sub></td><td align="center"><sup>1</sup>/<sub>3</sub></td><td align="center">1</td><td align="center">6</td></tr><tr><td align="center">Примеры</td><td align="center"><sup>1</sup>/<sub>3</sub></td><td align="center"><sup>1</sup>/<sub>4</sub></td><td align="center"><sup>1</sup>/<sub>5</sub></td><td align="center"><sup>1</sup>/<sub>6</sub></td><td align="center">1</td></tr></tbody></table>

Нормированный собственный вектор: W=(0.439; 0.298; 0.117; 0.0976; 0.0488)  
λmax=6.3
![](../Files/Pasted%20image%2020211222211711.png)
ОС=0.325/1.12=0.29  
Матрица для наличие лицензии

<table class="table table-bordered table-center"><tbody><tr><td align="center"> </td><td align="center">JADE</td><td align="center">MadKIT</td><td align="center">AgentBuilder</td><td align="center">Cougaar</td><td align="center">NetLogo</td><td align="center">VisualBots</td><td align="center">MASON</td></tr><tr><td align="center">JADE</td><td align="center">1</td><td align="center">7</td><td align="center">3</td><td align="center">8</td><td align="center">8</td><td align="center">5</td><td align="center">9</td></tr><tr><td align="center">MadKIT</td><td align="center"><sup>1</sup>/<sub>7</sub></td><td align="center">1</td><td align="center">9</td><td align="center">7</td><td align="center">1</td><td align="center">3</td><td align="center">7</td></tr><tr><td align="center">AgentBuilder</td><td align="center"><sup>1</sup>/<sub>3</sub></td><td align="center"><sup>1</sup>/<sub>9</sub></td><td align="center">1</td><td align="center">9</td><td align="center">2</td><td align="center">1</td><td align="center">6</td></tr><tr><td align="center">Cougaar</td><td align="center"><sup>1</sup>/<sub>8</sub></td><td align="center"><sup>1</sup>/<sub>7</sub></td><td align="center"><sup>1</sup>/<sub>9</sub></td><td align="center">1</td><td align="center">9</td><td align="center">2</td><td align="center">2</td></tr><tr><td align="center">NetLogo</td><td align="center"><sup>1</sup>/<sub>8</sub></td><td align="center">1</td><td align="center"><sup>1</sup>/<sub>2</sub></td><td align="center"><sup>1</sup>/<sub>9</sub></td><td align="center">1</td><td align="center">1</td><td align="center">9</td></tr><tr><td align="center">VisualBots</td><td align="center"><sup>1</sup>/<sub>5</sub></td><td align="center"><sup>1</sup>/<sub>3</sub></td><td align="center">1</td><td align="center"><sup>1</sup>/<sub>2</sub></td><td align="center">1</td><td align="center">1</td><td align="center">7</td></tr><tr><td align="center">MASON</td><td align="center"><sup>1</sup>/<sub>9</sub></td><td align="center"><sup>1</sup>/<sub>7</sub></td><td align="center"><sup>1</sup>/<sub>6</sub></td><td align="center"><sup>1</sup>/<sub>2</sub></td><td align="center"><sup>1</sup>/<sub>9</sub></td><td align="center"><sup>1</sup>/<sub>7</sub></td><td align="center">1</td></tr></tbody></table>

Собственный вектор: V=(23.2; 14; 8; 5; 4; 3.2; 1)  
Нормированный собственный вектор: W=(0.397; 0.24; 0.137; 0.0856; 0.0685; 0.0548; 0.0171)  
λmax=10
![](../Files/Pasted%20image%2020211222211744.png)
ОС=0.5/1.32=0.379  
Матрица для поддержка языка Java

<table class="table table-bordered table-center"><tbody><tr><td align="center"> </td><td align="center">JADE</td><td align="center">MadKIT</td><td align="center">AgentBuilder</td><td align="center">Cougaar</td><td align="center">NetLogo</td><td align="center">VisualBots</td><td align="center">MASON</td></tr><tr><td align="center">JADE</td><td align="center">1</td><td align="center">2</td><td align="center">3</td><td align="center">8</td><td align="center">6</td><td align="center">6</td><td align="center">7</td></tr><tr><td align="center">MadKIT</td><td align="center"><sup>1</sup>/<sub>2</sub></td><td align="center">1</td><td align="center">4</td><td align="center">5</td><td align="center">9</td><td align="center">1</td><td align="center">8</td></tr><tr><td align="center">AgentBuilder</td><td align="center"><sup>1</sup>/<sub>3</sub></td><td align="center"><sup>1</sup>/<sub>4</sub></td><td align="center">1</td><td align="center">4</td><td align="center">2</td><td align="center">2</td><td align="center">4</td></tr><tr><td align="center">Cougaar</td><td align="center"><sup>1</sup>/<sub>8</sub></td><td align="center"><sup>1</sup>/<sub>5</sub></td><td align="center"><sup>1</sup>/<sub>4</sub></td><td align="center">1</td><td align="center">8</td><td align="center">3</td><td align="center">1</td></tr><tr><td align="center">NetLogo</td><td align="center"><sup>1</sup>/<sub>6</sub></td><td align="center"><sup>1</sup>/<sub>9</sub></td><td align="center"><sup>1</sup>/<sub>2</sub></td><td align="center"><sup>1</sup>/<sub>8</sub></td><td align="center">1</td><td align="center">2</td><td align="center">4</td></tr><tr><td align="center">VisualBots</td><td align="center"><sup>1</sup>/<sub>6</sub></td><td align="center">1</td><td align="center"><sup>1</sup>/<sub>2</sub></td><td align="center"><sup>1</sup>/<sub>3</sub></td><td align="center"><sup>1</sup>/<sub>2</sub></td><td align="center">1</td><td align="center">4</td></tr><tr><td align="center">MASON</td><td align="center"><sup>1</sup>/<sub>7</sub></td><td align="center"><sup>1</sup>/<sub>8</sub></td><td align="center"><sup>1</sup>/<sub>4</sub></td><td align="center">1</td><td align="center"><sup>1</sup>/<sub>4</sub></td><td align="center"><sup>1</sup>/<sub>4</sub></td><td align="center">1</td></tr></tbody></table>

Собственный вектор: VMadKIT=11; 8.1; 4; 3.2; 2; 2.2; 1  
Нормированный собственный вектор: WMadKIT=0.349; 0.257; 0.127; 0.102; 0.0635; 0.0698; 0.0317  
λmax=9
![](../Files/Pasted%20image%2020211222212042.png)
ОС=0.333/1.32=0.252  
Матрица для оздание приложение под Android
<table class="table table-bordered table-center"><tbody><tr><td align="center"> </td><td align="center">JADE</td><td align="center">MadKIT</td><td align="center">AgentBuilder</td><td align="center">Cougaar</td><td align="center">NetLogo</td><td align="center">VisualBots</td><td align="center">MASON</td></tr><tr><td align="center">JADE</td><td align="center">1</td><td align="center">1</td><td align="center">7</td><td align="center">9</td><td align="center">5</td><td align="center">1</td><td align="center">3</td></tr><tr><td align="center">MadKIT</td><td align="center">1</td><td align="center">1</td><td align="center">5</td><td align="center">9</td><td align="center">2</td><td align="center">8</td><td align="center">4</td></tr><tr><td align="center">AgentBuilder</td><td align="center"><sup>1</sup>/<sub>7</sub></td><td align="center"><sup>1</sup>/<sub>5</sub></td><td align="center">1</td><td align="center">8</td><td align="center">6</td><td align="center">5</td><td align="center">7</td></tr><tr><td align="center">Cougaar</td><td align="center"><sup>1</sup>/<sub>9</sub></td><td align="center"><sup>1</sup>/<sub>9</sub></td><td align="center"><sup>1</sup>/<sub>8</sub></td><td align="center">1</td><td align="center">7</td><td align="center">8</td><td align="center">2</td></tr><tr><td align="center">NetLogo</td><td align="center"><sup>1</sup>/<sub>5</sub></td><td align="center"><sup>1</sup>/<sub>2</sub></td><td align="center"><sup>1</sup>/<sub>6</sub></td><td align="center"><sup>1</sup>/<sub>7</sub></td><td align="center">1</td><td align="center">4</td><td align="center">9</td></tr><tr><td align="center">VisualBots</td><td align="center">1</td><td align="center"><sup>1</sup>/<sub>8</sub></td><td align="center"><sup>1</sup>/<sub>5</sub></td><td align="center"><sup>1</sup>/<sub>8</sub></td><td align="center"><sup>1</sup>/<sub>4</sub></td><td align="center">1</td><td align="center">6</td></tr><tr><td align="center">MASON</td><td align="center"><sup>1</sup>/<sub>3</sub></td><td align="center"><sup>1</sup>/<sub>4</sub></td><td align="center"><sup>1</sup>/<sub>7</sub></td><td align="center"><sup>1</sup>/<sub>2</sub></td><td align="center"><sup>1</sup>/<sub>9</sub></td><td align="center"><sup>1</sup>/<sub>6</sub></td><td align="center">1</td></tr></tbody></table>

Собственный вектор: V=11.2; 11; 7; 4; 3; 2; 1  
Нормированный собственный вектор: W=0.286; 0.281; 0.179; 0.102; 0.0765; 0.051; 0.0255  
λmax=11
![](../Files/Pasted%20image%2020211222212120.png)
ОС=0.667/1.32=0.505  
Матрица для Наличие документации

<table class="table table-bordered table-center"><tbody><tr><td align="center"> </td><td align="center">JADE</td><td align="center">MadKIT</td><td align="center">AgentBuilder</td><td align="center">Cougaar</td><td align="center">NetLogo</td><td align="center">VisualBots</td><td align="center">MASON</td></tr><tr><td align="center">JADE</td><td align="center">1</td><td align="center">4</td><td align="center">8</td><td align="center">5</td><td align="center">8</td><td align="center">6</td><td align="center">6</td></tr><tr><td align="center">MadKIT</td><td align="center"><sup>1</sup>/<sub>4</sub></td><td align="center">1</td><td align="center">9</td><td align="center">3</td><td align="center">3</td><td align="center">6</td><td align="center">8</td></tr><tr><td align="center">AgentBuilder</td><td align="center"><sup>1</sup>/<sub>8</sub></td><td align="center"><sup>1</sup>/<sub>9</sub></td><td align="center">1</td><td align="center">4</td><td align="center">4</td><td align="center">3</td><td align="center">4</td></tr><tr><td align="center">Cougaar</td><td align="center"><sup>1</sup>/<sub>5</sub></td><td align="center"><sup>1</sup>/<sub>3</sub></td><td align="center"><sup>1</sup>/<sub>4</sub></td><td align="center">1</td><td align="center">3</td><td align="center">7</td><td align="center">3</td></tr><tr><td align="center">NetLogo</td><td align="center"><sup>1</sup>/<sub>8</sub></td><td align="center"><sup>1</sup>/<sub>3</sub></td><td align="center"><sup>1</sup>/<sub>4</sub></td><td align="center"><sup>1</sup>/<sub>3</sub></td><td align="center">1</td><td align="center">8</td><td align="center">4</td></tr><tr><td align="center">VisualBots</td><td align="center"><sup>1</sup>/<sub>6</sub></td><td align="center"><sup>1</sup>/<sub>6</sub></td><td align="center"><sup>1</sup>/<sub>3</sub></td><td align="center"><sup>1</sup>/<sub>7</sub></td><td align="center"><sup>1</sup>/<sub>8</sub></td><td align="center">1</td><td align="center">3</td></tr><tr><td align="center">MASON</td><td align="center"><sup>1</sup>/<sub>6</sub></td><td align="center"><sup>1</sup>/<sub>8</sub></td><td align="center"><sup>1</sup>/<sub>4</sub></td><td align="center"><sup>1</sup>/<sub>3</sub></td><td align="center"><sup>1</sup>/<sub>4</sub></td><td align="center"><sup>1</sup>/<sub>3</sub></td><td align="center">1</td></tr></tbody></table>

Собственный вектор: V=17.4; 11; 5; 4; 3; 1.2; 1  
Нормированный собственный вектор: W=0.408; 0.258; 0.117; 0.0939; 0.0704; 0.0282; 0.0235  
λmax=9
![](../Files/Pasted%20image%2020211222212155.png)
ОС=0.333/1.32=0.252  
Матрица для Примеры

<table class="table table-bordered table-center"><tbody><tr><td align="center"> </td><td align="center">JADE</td><td align="center">MadKIT</td><td align="center">AgentBuilder</td><td align="center">Cougaar</td><td align="center">NetLogo</td><td align="center">VisualBots</td><td align="center">MASON</td></tr><tr><td align="center">JADE</td><td align="center">1</td><td align="center">6</td><td align="center">6</td><td align="center">4</td><td align="center">3</td><td align="center">5</td><td align="center">6</td></tr><tr><td align="center">MadKIT</td><td align="center"><sup>1</sup>/<sub>6</sub></td><td align="center">1</td><td align="center">7</td><td align="center">3</td><td align="center">8</td><td align="center">8</td><td align="center">5</td></tr><tr><td align="center">AgentBuilder</td><td align="center"><sup>1</sup>/<sub>6</sub></td><td align="center"><sup>1</sup>/<sub>7</sub></td><td align="center">1</td><td align="center">9</td><td align="center">9</td><td align="center">7</td><td align="center">1</td></tr><tr><td align="center">Cougaar</td><td align="center"><sup>1</sup>/<sub>4</sub></td><td align="center"><sup>1</sup>/<sub>3</sub></td><td align="center"><sup>1</sup>/<sub>9</sub></td><td align="center">1</td><td align="center">3</td><td align="center">7</td><td align="center">9</td></tr><tr><td align="center">NetLogo</td><td align="center"><sup>1</sup>/<sub>3</sub></td><td align="center"><sup>1</sup>/<sub>8</sub></td><td align="center"><sup>1</sup>/<sub>9</sub></td><td align="center"><sup>1</sup>/<sub>3</sub></td><td align="center">1</td><td align="center">2</td><td align="center">1</td></tr><tr><td align="center">VisualBots</td><td align="center"><sup>1</sup>/<sub>5</sub></td><td align="center"><sup>1</sup>/<sub>8</sub></td><td align="center"><sup>1</sup>/<sub>7</sub></td><td align="center"><sup>1</sup>/<sub>7</sub></td><td align="center"><sup>1</sup>/<sub>2</sub></td><td align="center">1</td><td align="center">6</td></tr><tr><td align="center">MASON</td><td align="center"><sup>1</sup>/<sub>6</sub></td><td align="center"><sup>1</sup>/<sub>5</sub></td><td align="center">1</td><td align="center"><sup>1</sup>/<sub>9</sub></td><td align="center">1</td><td align="center"><sup>1</sup>/<sub>6</sub></td><td align="center">1</td></tr></tbody></table>

Собственный вектор: V=10.2; 7; 5; 3; 1; 1.1; 1  
Нормированный собственный вектор: W=0.36; 0.247; 0.177; 0.106; 0.0353; 0.0389; 0.0353  
λmax=10.3
![](../Files/Pasted%20image%2020211222212243.png)
ОС=0.55/1.32=0.417  
3. Осуществляем иерархический синтез. Последовательно определяем вектора приоритетов альтернатив WEA относительно элементов Eji, находящихся на всех иерархических уровнях. Вычисление векторов приоритетов проводится в направлении от нижних уровней к верхним с учетом конкретных связей между элементами, принадлежащими различным уровням. Вычисление производится путем перемножения соответствующих векторов и матриц.

<table><tbody><tr><td><table><tbody><tr><td><table class="table table-bordered"><tbody><tr><td>0,397</td><td>0,349</td><td>0,286</td><td>0,408</td><td>0,36</td></tr><tr><td>0,24</td><td>0,257</td><td>0,281</td><td>0,258</td><td>0,247</td></tr><tr><td>0,137</td><td>0,127</td><td>0,179</td><td>0,117</td><td>0,177</td></tr><tr><td>0,0856</td><td>0,102</td><td>0,102</td><td>0,0939</td><td>0,106</td></tr><tr><td>0,0685</td><td>0,0635</td><td>0,0765</td><td>0,0704</td><td>0,0353</td></tr><tr><td>0,0548</td><td>0,0698</td><td>0,051</td><td>0,0282</td><td>0,0389</td></tr><tr><td>0,0171</td><td>0,0317</td><td>0,0255</td><td>0,0235</td><td>0,0353</td></tr></tbody></table></td><td></td></tr></tbody></table></td><td><table><tbody><tr><td><table class="table table-bordered"><tbody><tr><td>0,439</td></tr><tr><td>0,298</td></tr><tr><td>0,117</td></tr><tr><td>0,0976</td></tr><tr><td>0,0488</td></tr></tbody></table></td><td></td></tr></tbody></table></td><td>=</td><td><table><tbody><tr><td><table class="table table-bordered"><tbody><tr><td>0,3691358</td></tr><tr><td>0,2520574</td></tr><tr><td>0,1389888</td></tr><tr><td>0,09424584</td></tr><tr><td>0,06653868</td></tr><tr><td>0,05547524</td></tr><tr><td>0,02395324</td></tr></tbody></table></td><td></td></tr></tbody></table></td><td>
</td></tr></tbody></table>

Максимальным элементом в матрице является 0.369. Следовательно, наиболее важным параметром при выборе будет являться JADE

<h5 align="center">Вывод:</h5>
провёл сравнительный анализ средств разработки ИС анализа иерархий Т. Саати.



