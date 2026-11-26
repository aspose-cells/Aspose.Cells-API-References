---
title: "ThreeDFormat.BottomBevelWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThreeDFormat. Получает и задает ширину нижней фаски или насколько глубоко она применяется к фигуре. В единицах пунктов"
type: docs
url: /ru/net/aspose.cells.drawing/threedformat/bottombevelwidth/
---
## ThreeDFormat.BottomBevelWidth property

Получает и задает ширину нижнего скоса, или насколько глубоко он применяется к фигуре. В единицах точек.

```csharp
public double BottomBevelWidth { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyBottomBevelWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 100, 100);
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            threeDFormat.BottomBevelType = BevelType.ArtDeco;
            threeDFormat.BottomBevelWidth = 15;
            threeDFormat.BottomBevelHeight = 8;

            workbook.Save("ThreeDFormatBottomBevelDemo.xlsx");
        }
    }
}
```

### См. также

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


