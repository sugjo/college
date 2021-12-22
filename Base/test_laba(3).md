---
tags:
- тестирование
- лаба
---
<h5 align="center">Лабораторная работа № 3</h5>

<h5 align="center">Ручная отладка программного обеспечения</h5>

**Цель работы:** 
Ознакомиться с ручной отладкой ПО

<h5 align="center">Ход работы:</h5>

![](../Files/Pasted%20image%2020211222215950.png)

```JS
function getTriangleType(x, y, z) {
	return +(
		((2 * Math.cos(x - Math.PI / 6)) / (0.5 + Math.sin(y) ** 2)) *
        (1 + z ** 2 / (3 - z ** 2 / 5))
      ).toFixed(2);
}
```

```JS
const inquirer = require('inquirer')
const calculate = require("./calculate");

inquirer
    .prompt([
        { type: "number", message: "Введите x:", default: 0, name: "x" },
        { type: "number", message: "Введите y:", default: 0, name: "y" },
        { type: "number", message: "Введите z:", default: 0, name: "z" },
    ])
    .then((answers) => {
        console.log(calculate(answers.x, answers.y, answers.z)); //
    })
    .catch((error) => {
        console.log(error);
    });
```

![](../Files/my%20test%20code.png)
![](../Files/my%20test.png)