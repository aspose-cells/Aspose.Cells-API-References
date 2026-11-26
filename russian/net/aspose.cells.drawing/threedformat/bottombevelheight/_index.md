---
title: "ThreeDFormat.BottomBevelHeight"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreeDFormat. Получает и задает высоту нижней фаски или глубину её применения к фигуре. В единицах точек"
type: docs
url: /ru/net/aspose.cells.drawing/threedformat/bottombevelheight/
---
## ThreeDFormat.BottomBevelHeight property

Получает и задает высоту нижнего скоса, или насколько глубоко он применяется к фигуре. В единицах точек.

```csharp
public double BottomBevelHeight { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyBottomBevelHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 100, 100);
            
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.BottomBevelType = BevelType.Circle;
            threeDFormat.BottomBevelWidth = 8;
            threeDFormat.BottomBevelHeight = 12;

            workbook.Save("ThreeDFormatBottomBevelDemo.xlsx");
        }
    }
}
```

### См. также

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


