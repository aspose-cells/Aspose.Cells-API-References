---
title: "ThreeDFormat.TopBevelWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreeDFormat egenskap. Hämtar och anger bredden på den övre fasetten eller hur långt in i formen den tillämpas. I enhet av punkter"
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/topbevelwidth/
---
## ThreeDFormat.TopBevelWidth property

Hämtar och anger bredden på den övre fasen, eller hur långt in i formen den appliceras. I enheten punkter.

```csharp
public double TopBevelWidth { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyTopBevelWidthDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet med korrekta parametrar
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 0, 0);

            // Hämta 3D-formatet för formen
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Ställ in 3D-egenskaper inklusive TopBevelWidth
            threeDFormat.TopBevelType = BevelType.HardEdge;
            threeDFormat.TopBevelWidth = 30;
            threeDFormat.TopBevelHeight = 30;
            threeDFormat.ContourWidth = 17;
            threeDFormat.ExtrusionHeight = 32;

            // Spara arbetsboken
            workbook.Save("ThreeDFormatDemo.xlsx");

            // Verifiera de sparade egenskaperna
            Workbook loadedWorkbook = new Workbook("ThreeDFormatDemo.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ThreeDFormat loadedFormat = loadedShape.ThreeDFormat;

            Console.WriteLine("TopBevelWidth: " + loadedFormat.TopBevelWidth);
            Console.WriteLine("TopBevelHeight: " + loadedFormat.TopBevelHeight);
            Console.WriteLine("TopBevelType: " + loadedFormat.TopBevelType);
            Console.WriteLine("ContourWidth: " + loadedFormat.ContourWidth);
            Console.WriteLine("ExtrusionHeight: " + loadedFormat.ExtrusionHeight);
        }
    }
}
```

### Se även

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


