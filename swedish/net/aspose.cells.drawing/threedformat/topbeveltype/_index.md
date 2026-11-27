---
title: "ThreeDFormat.TopBevelType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreeDFormat-egenskap. Hämtar och anger typen av toppavfasning eller hur djupt den appliceras på formen. I enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/topbeveltype/
---
## ThreeDFormat.TopBevelType property

Hämtar och anger typen av den övre fasen, eller hur långt in i formen den appliceras. I enheten punkter.

```csharp
public BevelType TopBevelType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyTopBevelTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 100, 100);
            
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.TopBevelType = BevelType.SoftRound;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;

            workbook.Save("ThreeDFormatTopBevelDemo.xlsx");
        }
    }
}
```

### Se även

* enum [BevelType](../../beveltype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


