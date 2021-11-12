---
tags:
- разработка
- лаба
---
<h5 align="center">Лабораторная работа № 22-23</h5>

<h5 align="center"></h5>

**Цель работы:** 

<h5 align="center">Теория</h5>



<h5 align="center">Ход работы:</h5>

8. Найти произведение k квадратных матриц A1, A2,…, Ak. Функция: вычисление произведения двух матриц.

```C#
int k = Convert.ToInt32(Console.ReadLine());
Console.WriteLine();
Random random = new Random();
int[,] matrix = new int[3, 3];

matrix = pullMatrix();

multiplyMatrix(ref matrix);

void multiplyMatrix(ref int[,] _matrix)
{
    int[,] arr = new int[3, 3];
    arr = pullMatrix();

    for (int i = 0; i < 3; i++)
    {
        for (int j = 0; j < 3; j++)
        {
            _matrix[i, j] += arr[i, j];
            Console.Write($"{_matrix[i, j]}\t");
        }
        Console.WriteLine();
    }
    Console.WriteLine();
    k--;
    if (k <= 1)
        return;
    multiplyMatrix(ref _matrix);
} //Складывание матриц

int[,] pullMatrix()
{
    int[,] array = new int[3, 3];
    for (int i = 0; i < 3; i++)
    {
        for (int j = 0; j < 3; j++)
        {
            array[i,j] = random.Next(0, 9);
            Console.Write($"{array[i, j]}\t");
        }
        Console.WriteLine();
    }
    Console.WriteLine();
    return array;
} //Заполнить матрицу и показать матрицу

Console.ReadKey();
```

выполнение:
![](../Files/Pasted%20image%2020211106151249.png)

<h5 align="center">Контрольные вопросы:</h5>


