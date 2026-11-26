---
title: "Shape.WidthInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет ширину фигуры в дюймах"
type: docs
url: /ru/net/aspose.cells.drawing/shape/widthinch/
---
## Shape.WidthInch property

Представляет ширину фигуры в дюймах.

```csharp
public double WidthInch { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // Установить ширину в дюймах
            shape.WidthInch = 3;
            Console.WriteLine("Shape width (inches): " + shape.WidthInch);

            // Изменить ширину, если условие выполнено
            if (shape.WidthInch == 3)
            {
                shape.WidthInch = 1;
                Console.WriteLine("Modified shape width (inches): " + shape.WidthInch);
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


