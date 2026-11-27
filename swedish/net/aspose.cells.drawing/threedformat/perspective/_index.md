---
title: "ThreeDFormat.Perspective"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreeDFormat egenskap. Hämtar och anger vinkeln där ett ThreeDFormat-objekt kan ses"
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/perspective/
---
## ThreeDFormat.Perspective property

Hämtar och anger vinkeln vid vilken ett ThreeDFormat-objekt kan visas.

```csharp
public double Perspective { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyPerspectiveDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera 3D-formatering
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 0, 0, 200, 100);
            
            // Hämta 3D-formatet för formen
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Visa aktuellt perspektivvärde
            Console.WriteLine("Current Perspective value: " + threeDFormat.Perspective);

            // Ställ in nytt perspektivvärde (0 till 120 grader)
            threeDFormat.Perspective = 45;
            Console.WriteLine("Perspective set to: " + threeDFormat.Perspective);

            // Applicera andra 3D-effekter för att bättre visualisera perspektivändringen
            threeDFormat.ExtrusionHeight = 15;
            threeDFormat.ContourWidth = 2;
            threeDFormat.RotationX = 20;
            threeDFormat.RotationY = 30;

            // Spara arbetsboken för att se effekterna
            workbook.Save("ThreeDFormatPerspectiveDemo.xlsx");
        }
    }
}
```

### Se även

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


