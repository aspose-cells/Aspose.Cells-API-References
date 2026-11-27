---
title: "ThreeDFormat.BottomBevelWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreeDFormat egenskap. Hämtar och anger bredden på den nedre fasetten eller hur långt in i formen den tillämpas. I enhet av punkter"
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/bottombevelwidth/
---
## ThreeDFormat.BottomBevelWidth property

Hämtar och anger bredden på den nedre fasen, eller hur långt in i formen den tillämpas. I enheten Points.

```csharp
public double BottomBevelWidth { get; set; }
```

### Exempel

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

### Se även

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


