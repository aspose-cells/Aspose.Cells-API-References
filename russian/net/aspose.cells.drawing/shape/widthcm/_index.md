---
title: "Shape.WidthCM"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет ширину фигуры в сантиметрах"
type: docs
url: /ru/net/aspose.cells.drawing/shape/widthcm/
---
## Shape.WidthCM property

Представляет ширину фигуры в сантиметрах.

```csharp
public double WidthCM { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWidthCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить прямоугольную фигуру
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 100, 100);

            // Установить ширину в сантиметрах
            shape.WidthCM = 3.5;
            Console.WriteLine("Shape width set to: " + shape.WidthCM + " cm");

            // Изменить ширину, если она соответствует условию
            if (shape.WidthCM == 3.5)
            {
                shape.WidthCM = 2.0;
                Console.WriteLine("Shape width changed to: " + shape.WidthCM + " cm");
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


