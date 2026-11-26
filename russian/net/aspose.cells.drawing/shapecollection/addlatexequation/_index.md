---
title: "ShapeCollection.AddLaTeXEquation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет объект уравнения в лист, используя строки в формате LaTeX"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addlatexequation/
---
## ShapeCollection.AddLaTeXEquation method

Добавляет объект уравнения на лист, используя строки в формате LaTeX.

```csharp
public TextBox AddLaTeXEquation(int topRow, int top, int leftColumn, int left, int height, 
    int width, string latex)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс верхней строки. |
| верх | Int32 | Вертикальное смещение его верхней строки в пикселях. |
| leftColumn | Int32 | Индекс левой колонки. |
| влево | Int32 | Горизонтальное смещение от её левой колонки, в пикселях. |
| высота | Int32 | Высота уравнения, в пикселях. |
| ширина | Int32 | Ширина уравнения, в пикселях. |
| latex | String | Строка формата LaTeX |

### Примеры

```csharp

[C#]
// Строка формата LaTeX.
string latex = "\\alpha +  \\frac{\\partial^2}{\\partial x_1\\partial x_2}y - \\left ( a + b \\right )+_{a}^{b}\\beta";
// Добавляет объект уравнения на лист.
TextBox textBox = shapes.AddLaTeXEquation(1, 0, 1, 0, 100, 300, latex);
```

### См. также

* class [TextBox](../../textbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


