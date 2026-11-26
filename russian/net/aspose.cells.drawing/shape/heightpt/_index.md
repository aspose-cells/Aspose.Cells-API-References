---
title: "Shape.HeightPt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Shape. Представляет высоту формы в единицах пунктов"
type: docs
url: /ru/net/aspose.cells.drawing/shape/heightpt/
---
## Shape.HeightPt property

Представляет высоту фигуры в пунктах.

```csharp
public double HeightPt { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHeightPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте образец фигуры со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 100);

            // Установить и получить свойство HeightPt
            shape.HeightPt = 50;
            Console.WriteLine("Shape height in points: " + shape.HeightPt);

            // Изменить высоту, если она соответствует условию
            if (shape.HeightPt == 50)
            {
                shape.HeightPt = 30;
                Console.WriteLine("Modified shape height: " + shape.HeightPt);
            }
        }
    }
}
```

### См. также

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


