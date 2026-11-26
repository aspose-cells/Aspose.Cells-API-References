---
title: "Shape.LeftInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет горизонтальное смещение фигуры от её левого столбца в дюймах"
type: docs
url: /ru/net/aspose.cells.drawing/shape/leftinch/
---
## Shape.LeftInch property

Представляет горизонтальное смещение фигуры от её левого столбца в дюймах.

```csharp
public double LeftInch { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLeftInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образец фигуры со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Установить и продемонстрировать свойство LeftInch
            shape.LeftInch = 3;
            Console.WriteLine("Shape left position (inches): " + shape.LeftInch);

            // Изменить левое положение, если оно 3 дюйма
            if (shape.LeftInch == 3)
            {
                shape.LeftInch = 1;
                Console.WriteLine("Adjusted shape left position (inches): " + shape.LeftInch);
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


