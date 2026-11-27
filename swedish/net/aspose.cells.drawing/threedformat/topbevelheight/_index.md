---
title: "ThreeDFormat.TopBevelHeight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreeDFormat-egenskap. Hämtar och anger höjden på den övre fasen eller hur långt in i formen den tillämpas. I enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/topbevelheight/
---
## ThreeDFormat.TopBevelHeight property

Hämtar och anger höjden på den övre fasen, eller hur långt in i formen den appliceras. I enheten punkter.

```csharp
public double TopBevelHeight { get; set; }
```

### Exempel

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

### Se även

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


