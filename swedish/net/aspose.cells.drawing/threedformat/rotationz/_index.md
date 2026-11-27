---
title: "ThreeDFormat.RotationZ"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreeDFormat egenskap. Hämtar och anger rotationen av den extruderade formen kring z-axeln i grader"
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/rotationz/
---
## ThreeDFormat.RotationZ property

Hämtar och anger rotationen av den extruderade formen runt z-axeln i grader.

```csharp
public double RotationZ { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationZDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera 3D-formatering
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 0, 2, 0, 100, 150);
            shape.Text = "3D Rotation Demo";
            
            // Åtkomst till ThreeDFormat för formen
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Visa aktuellt RotationZ‑värde
            Console.WriteLine("Current RotationZ value: " + threeDFormat.RotationZ);

            // Ange nya RotationZ‑värden och demonstrera effekterna
            threeDFormat.RotationZ = 45;
            Console.WriteLine("Shape rotated 45 degrees around Z-axis");

            // Applicera andra 3D‑egenskaper för att göra rotationen synlig
            threeDFormat.ExtrusionHeight = 15;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.OrthographicFront;

            // Spara arbetsboken med 3D‑effekterna
            workbook.Save("ThreeDFormatRotationZDemo.xlsx");
        }
    }
}
```

### Se även

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


