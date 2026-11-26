---
title: "ThreeDFormat.TopBevelHeight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreeDFormat. Получает и задает высоту верхней фаски или глубину её применения к фигуре. В единицах точек"
type: docs
url: /ru/net/aspose.cells.drawing/threedformat/topbevelheight/
---
## ThreeDFormat.TopBevelHeight property

Получает и задает высоту верхнего скоса, или насколько глубоко он применяется к фигуре. В единицах точек.

```csharp
public double TopBevelHeight { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyTopBevelHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 100, 100);
            
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.TopBevelType = BevelType.Circle;
            threeDFormat.TopBevelHeight = 15;
            threeDFormat.TopBevelWidth = 10;

            workbook.Save("ThreeDFormatTopBevelHeightDemo.xlsx");
        }
    }
}
```

### См. также

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


