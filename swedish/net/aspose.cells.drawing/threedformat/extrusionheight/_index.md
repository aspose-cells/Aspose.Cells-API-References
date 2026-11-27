---
title: "ThreeDFormat.ExtrusionHeight"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreeDFormat-egenskap. Hämtar och anger extrusionshöjden som tillämpas på formen i enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/extrusionheight/
---
## ThreeDFormat.ExtrusionHeight property

Hämtar och anger extruderingshöjden som tillämpas på formen, i enheten punkter.

```csharp
public double ExtrusionHeight { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyExtrusionHeightDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en exempelform med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Tillämpa 3D-formatering
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.ExtrusionHeight = 32;
            threeDFormat.ContourWidth = 17;
            threeDFormat.TopBevelType = BevelType.HardEdge;
            threeDFormat.TopBevelWidth = 30;
            threeDFormat.TopBevelHeight = 30;

            // Spara arbetsboken
            workbook.Save("output.xlsx");

            // Verifiera de sparade värdena
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ThreeDFormat loadedFormat = loadedShape.ThreeDFormat;

            Console.WriteLine("ExtrusionHeight: " + loadedFormat.ExtrusionHeight);
            Console.WriteLine("ContourWidth: " + loadedFormat.ContourWidth);
            Console.WriteLine("TopBevelType: " + loadedFormat.TopBevelType);
            Console.WriteLine("TopBevelWidth: " + loadedFormat.TopBevelWidth);
            Console.WriteLine("TopBevelHeight: " + loadedFormat.TopBevelHeight);
        }
    }
}
```

### Se även

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


