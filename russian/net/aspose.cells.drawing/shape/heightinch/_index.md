---
title: "Shape.HeightInch"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет высоту формы в единицах дюймов"
type: docs
url: /ru/net/aspose.cells.drawing/shape/heightinch/
---
## Shape.HeightInch property

Представляет высоту фигуры в дюймах.

```csharp
public double HeightInch { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте прямоугольную форму со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 100);

            // Задайте и получите высоту в дюймах
            shape.HeightInch = 3;
            Console.WriteLine("Shape height (inches): " + shape.HeightInch);

            // Измените высоту, если условие выполнено
            if (shape.HeightInch == 3)
            {
                shape.HeightInch = 1;
                Console.WriteLine("Modified shape height (inches): " + shape.HeightInch);
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


