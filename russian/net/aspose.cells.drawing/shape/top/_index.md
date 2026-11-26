---
title: "Shape.Top"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет вертикальное смещение формы от её верхней строки в пикселях"
type: docs
url: /ru/net/aspose.cells.drawing/shape/top/
---
## Shape.Top property

Представляет вертикальное смещение фигуры от её верхней строки в пикселях.

```csharp
public int Top { get; set; }
```

### Примечания

Если фигура находится в диаграмме, представляет вертикальное смещение фигуры от её верхней границы.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Установите начальное верхнее положение
            shape.Top = 50;
            Console.WriteLine("Initial Top position: " + shape.Top);

            // Измените верхнее положение, если оно равно 3 (демонстрация логики тестового случая)
            if (shape.Top == 3)
            {
                shape.Top = 1;
            }
            else
            {
                // Для демонстрации установите значение 3, а затем примените логику тестового случая
                shape.Top = 3;
                if (shape.Top == 3)
                {
                    shape.Top = 1;
                    Console.WriteLine("Modified Top position: " + shape.Top);
                }
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


