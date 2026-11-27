---
title: "ThreeDFormat.RotationY"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreeDFormat-egenskap. Hämtar och anger rotationen av den extruderade formen runt y-axeln i grader"
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/rotationy/
---
## ThreeDFormat.RotationY property

Hämtar och anger rotationen av den extruderade formen runt y-axeln i grader.

```csharp
public double RotationY { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyRotationYDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera 3D-formatering
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 0, 2, 100, 150, 150);
            shape.Text = "3D Rotation Demo";
            
            // Åtkomst till ThreeDFormat för formen
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Visa aktuellt RotationY-värde
            Console.WriteLine("Current RotationY value: " + threeDFormat.RotationY);

            // Ange nya RotationY-värden och demonstrera effekterna
            threeDFormat.RotationY = 15;
            Console.WriteLine("Shape rotated 15 degrees around Y-axis");

            // Tillämpa några andra 3D-egenskaper för att göra effekten synlig
            threeDFormat.ExtrusionHeight = 5;
            threeDFormat.ContourWidth = 1;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveContrastingRightFacing;

            // Spara arbetsboken för att visa effekterna
            workbook.Save("ThreeDFormatRotationYDemo.xlsx");

            // Ändra rotationen igen och spara en annan version
            threeDFormat.RotationY = 45;
            workbook.Save("ThreeDFormatRotationYDemo_45degrees.xlsx");
        }
    }
}
```

### Se även

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


