---
title: "ThreeDFormat.RotationX"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreeDFormat egenskap. Hämtar och anger rotationen av den extruderade formen kring x‑axeln i grader"
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/rotationx/
---
## ThreeDFormat.RotationX property

Hämtar och anger rotationen av den extruderade formen runt x-axeln i grader.

```csharp
public double RotationX { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationXDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera 3D-formatering
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 2, 2, 200, 100, 100);
            
            // Hämta 3D‑format (ingen anledning att "aktivera" 3D‑effekter – bara ange egenskaperna)
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Visa aktuellt RotationX‑värde
            Console.WriteLine("Current RotationX value: " + threeDFormat.RotationX);

            // Ange nytt RotationX‑värde (rotation kring x‑axeln i grader)
            threeDFormat.RotationX = 45;
            Console.WriteLine("New RotationX value: " + threeDFormat.RotationX);

            // Ange andra 3D‑egenskaper för att göra rotationen synlig
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.OrthographicFront;

            // Spara arbetsboken för att se effekterna
            workbook.Save("ThreeDFormatRotationXDemo.xlsx");
        }
    }
}
```

### Se även

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


