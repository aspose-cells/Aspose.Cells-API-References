---
title: "ThreeDFormat.BottomBevelType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreeDFormat egenskap. Hämtar och anger typen av den nedre fasen eller hur långt in i formen den tillämpas. I enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/bottombeveltype/
---
## ThreeDFormat.BottomBevelType property

Hämtar och anger typen av den nedre fasen, eller hur långt in i formen den tillämpas. I enheten Points.

```csharp
public BevelType BottomBevelType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyBottomBevelTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 100, 100);
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            threeDFormat.BottomBevelType = BevelType.Divot;
            threeDFormat.BottomBevelWidth = 8;
            threeDFormat.BottomBevelHeight = 8;

            workbook.Save("ThreeDFormatBottomBevelDemo.xlsx");
        }
    }
}
```

### Se även

* enum [BevelType](../../beveltype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


