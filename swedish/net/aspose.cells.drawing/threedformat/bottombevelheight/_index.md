---
title: "ThreeDFormat.BottomBevelHeight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreeDFormat-egenskap. Hämtar och anger höjden på den nedre fasen eller hur långt in i formen den tillämpas. I enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/bottombevelheight/
---
## ThreeDFormat.BottomBevelHeight property

Hämtar och anger höjden på den nedre fasen, eller hur långt in i formen den tillämpas. I enheten Points.

```csharp
public double BottomBevelHeight { get; set; }
```

### Exempel

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

### Se även

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


