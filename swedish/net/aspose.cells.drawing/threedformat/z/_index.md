---
title: "ThreeDFormat.Z"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreeDFormat egenskap. Definierar avståndet från marken för den 3D‑formen"
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/z/
---
## ThreeDFormat.Z property

Definierar avståndet från marken för den 3D-formen.

```csharp
public double Z { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyZDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera 3D-formatering
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 0, 0, 200, 100);
            
            // Åtkomst till ThreeDFormat för formen
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Visa aktuellt Z‑värde (avstånd från marken)
            Console.WriteLine("Current Z value: " + threeDFormat.Z);

            // Ange nytt Z‑värde för att flytta formen längre bort från marken
            threeDFormat.Z = 20;
            Console.WriteLine("New Z value: " + threeDFormat.Z);

            // Konfigurera andra 3D‑egenskaper för att göra effekten synlig
            threeDFormat.ExtrusionHeight = 30;
            threeDFormat.ContourWidth = 2;
            threeDFormat.PresetCameraType = PresetCameraType.PerspectiveContrastingRightFacing;

            // Spara arbetsboken för att se 3D‑effekten
            workbook.Save("ThreeDFormatPropertyZDemo.xlsx");
        }
    }
}
```

### Se även

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


