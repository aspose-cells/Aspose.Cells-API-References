---
title: "Shape.X"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Получает и задает горизонтальное смещение формы от левого края листа в пикселях"
type: docs
url: /ru/net/aspose.cells.drawing/shape/x/
---
## Shape.X property

Получает и задает горизонтальное смещение фигуры от левой границы листа, в пикселях.

```csharp
public int X { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyXDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 0, 0);

            // Установить начальное положение X
            shape.X = 200;
            Console.WriteLine("Initial X position: " + shape.X);

            // Изменить положение X, если оно равно 3 (демонстрация логики тестового случая)
            if (shape.X == 3)
            {
                shape.X = 1;
            }
            else
            {
                // Для демонстрации изменить положение X на 300
                shape.X = 300;
            }

            Console.WriteLine("Final X position: " + shape.X);
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


