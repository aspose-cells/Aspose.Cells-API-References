---
title: "ThreeDFormat.ContourWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreeDFormat egenskap. Hämtar och anger konturens bredd på formen i enhet av punkter"
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/contourwidth/
---
## ThreeDFormat.ContourWidth property

Hämtar och anger konturbredden på formen, i enheten punkter.

```csharp
public double ContourWidth { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyContourWidthDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Lägg till en form i kalkylbladet med alla nödvändiga parametrar
            Shape sh = ws.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 100, 0, 0);

            // Tillämpa 3D-formatering
            ThreeDFormat n3df = sh.ThreeDFormat;
            n3df.ContourWidth = 17;
            n3df.ExtrusionHeight = 32;
            n3df.TopBevelType = (BevelType)BevelPresetType.HardEdge;

            // Spara arbetsboken
            wb.Save("output.xlsx");

            // Verifiera de sparade värdena
            Workbook wb2 = new Workbook("output.xlsx");
            Shape sh2 = wb2.Worksheets[0].Shapes[0];
            ThreeDFormat n3df2 = sh2.ThreeDFormat;

            Console.WriteLine("ContourWidth: " + n3df2.ContourWidth);
            Console.WriteLine("ExtrusionHeight: " + n3df2.ExtrusionHeight);
            Console.WriteLine("TopBevelType: " + n3df2.TopBevelType);
        }
    }
}
```

### Se även

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


