---
tags:
- разработка
- лаба
---
<h5 align="center">Лабораторная работа № 16-17</h5>

<h5 align="center">«Программная реализация циклического алгоритма. Цикл с предусловием»</h5>

**Цель работы:** 
получение навыков реализации циклического алгоритма, используя цикл с предусловием на языке С#.

<h5 align="center">Теория</h5>

Цикл с предусловием работает следующим образом. Вычисляется значение выражения. Если оно истинно, то выполняется оператор. В противном случае цикл заканчивается. Если состоит более чем из одного оператора, необходимо использовать составной оператор:

```C#
while(условие)
	оператор(операторы); 
```
	
где оператор - это единственный оператор или же блок операторов, а условие означает конкретное условие управления циклом и может быть любым логическим выражением. В этом цикле оператор выполняется до тех пор, пока условие истинно. Как только условие становится ложным, управление программой передается строке кода, следующей непосредственно после цикла.

Как и в цикле for, в цикле while проверяется условное выражение, указываемое в самом начале цикла. Это означает, что код в теле цикла может вообще не выполняться, а также избавляет от необходимости выполнять отдельную проверку перед самим циклом.

Пример:

```C#

// Пример возведения числа в несколько степеней

byte l = 2, i = 0;

int result = 1;

while (i < 10)

{

	i++;

	result *= l;

	Console.WriteLine("{0} в степени {1} равно {2}",l,i,result);

}
```

<h5 align="center">Ход работы:</h5>

4. Дано натуральное число n. Напишите программу, вычисляющую сумму цифр числа n. Выведите сумму цифр числа n.

```C#
string n = Convert.ToString(Console.ReadLine());
int i = 0;
int result = 0;

while (i < n.Length)
{
	result += int.Parse(Convert.ToString(n[i]));
    i++;
}

Console.WriteLine(result);
Console.ReadLine();
```
выполнение:
![](../Files/Pasted%20image%2020211104180413.png)
<h5 align="center">Контрольные вопросы:</h5>

1. Назначение оператора цикла с предусловием.
	- Как и в цикле for, в цикле while проверяется условное выражение, указываемое в самом начале цикла. Это означает, что код в теле цикла может вообще не выполняться, а также избавляет от необходимости выполнять отдельную проверку перед самим циклом.
2. Опишите синтаксис данного оператора.
```C#
while(условие)
	оператор(операторы); 
```
3. В чем разница между этим оператором и оператором цикла?
	- Единственное **отличие** заключается в способе записи цикла. Практически любой цикл `while` можно преобразовать в цикл `for`
4. Что такое бесконечный цикл?
	- **цикл**, написанный таким образом, что условие выхода из него никогда не выполняется.