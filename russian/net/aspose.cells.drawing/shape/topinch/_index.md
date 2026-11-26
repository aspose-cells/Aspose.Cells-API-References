---
title: "Shape.TopInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет вертикальное смещение формы от её верхней строки в дюймах"
type: docs
url: /ru/net/aspose.cells.drawing/shape/topinch/
---
## Shape.TopInch property

Представляет вертикальное смещение фигуры от её верхней строки в дюймах.

```csharp
public double TopInch { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTopInchDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);

            // Установите и продемонстрируйте свойство TopInch
            shape.TopInch = 3;
            Console.WriteLine("Shape Top position (inches): " + shape.TopInch);

            // Измените TopInch, если он равен 3
            if (shape.TopInch == 3)
            {
                shape.TopInch = 1;
                Console.WriteLine("Modified Shape Top position (inches): " + shape.TopInch);
            }

            // Сохраните книгу
            workbook.Save("ShapeTopInchDemo.xlsx");
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


