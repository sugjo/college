<h5 align="center">Лаботаторная работа № 2-3</h5>

<h5 align="center">«Оценка сложности и оформление алгоритмов линейной структуры»</h5>

 Тэги: #разработка #лаба

**Цель работы:** ознакомиться оператором ветвления и научиться составлять программы с его использованием.

Алгоритм линейной структуры - последовательность действий и не содержит каких-либо условий.
линейные алгоритмы выполняются в естественном порядке его написания и не содержит разветвлений и повторений.
![](../Files/image1.jpeg)
***Рисунок 1 – Последовательность действий***

На практике линейные алгоритмы в чистом виде встречаются редко
Даны катеты прямоугольного треугольника. Найти его периметр.
Листинг:

```c++
static void Main(string[] args)
{
 int a,b; double c,p;
 Console.WriteLine("Даны катеты прямоугольного треугольника. Найти его периметр.");
 Console.Write("Введите длину катета А=");
 a = Convert.ToInt32(Console.ReadLine());
 Console.Write("Введите длину катета B=");
 b = Convert.ToInt32(Console.ReadLine());
 c = Math.Sqrt(Math.Pow(a, 2) + Math.Pow(b, 2));
 Console.Write("Длина гипотенузы равна "+"{0:0.00}",c);
 Console.WriteLine();
 p = a + b + c;
 Console.Write("Периметр треугольника равен " + "{0:0.00}", p);
}

```
![](../Files/image2%201.png)

<h5 align="center">Ход работы:</h5>

4. Даны три действительных числа. Найти среднее арифметическое и среднее геометрическое их модулей.

код:
```js
const inquirer = require('inquirer');
inquirer
    .prompt([
        { type: 'number', message: 'Введите первое число:', name: 'a' },
        { type: 'number', message: 'Введите второе число:', name: 'b' },
        { type: 'number', message: 'Введите третье число:', name: 'c' },
        { type: 'number', message: 'округлить до:', name: 'round' }
    ])
    .then((answers) => {
        console.log(`среднее арифметическое: ${arithmeticMean(answers.a, answers.b, answers.c, answers.round)}`)
        console.log(`среднее геометрическое: ${geometricMean(answers.a, answers.b, answers.c, answers.round)}`)
    })
    .catch((error) => {
        console.log(error);
    });

function arithmeticMean(a, b, c, round) {
    a = Math.abs(a)
    b = Math.abs(b)
    c = Math.abs(c)
    return ((a + b + c) / 3).toFixed(round)
}

function geometricMean(a, b, c, round) {
    a = Math.abs(a)
    b = Math.abs(b)
    c = Math.abs(c)
    return Math.cbrt((a * b * c)).toFixed(round)
}
```
выполнение:
![](../Files/Pasted%20image%2020210924172819.png)