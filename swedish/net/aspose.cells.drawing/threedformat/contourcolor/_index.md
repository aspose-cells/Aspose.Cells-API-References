---
title: "ThreeDFormat.ContourColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreeDFormat-egenskap. Hämtar och anger konturfärgen på en form"
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/contourcolor/
---
## ThreeDFormat.ContourColor property

Hämtar och anger konturfärgen på en form.

```csharp
public CellsColor ContourColor { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyContourColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera 3D-formatering
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 200, 100, 0, 0);
            shape.Text = "3D ContourColor Demo";
            
            // Hämta ThreeDFormat för formen
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Konfigurera grundläggande 3D-egenskaper
            threeDFormat.TopBevelType = BevelType.ArtDeco;
            threeDFormat.TopBevelWidth = 10;
            threeDFormat.TopBevelHeight = 10;
            threeDFormat.ContourWidth = 2;

            try
            {
                // Hämta aktuellt ContourColor-värde
                CellsColor contourColor = threeDFormat.ContourColor;
                Console.WriteLine($"Initial ContourColor - Type: {contourColor.Type}, ARGB: {contourColor.Argb}");

                // Skapa ny färg genom att modifiera befintlig
                contourColor.Argb = System.Drawing.Color.Red.ToArgb();
                contourColor.Transparency = 0.5;
                threeDFormat.ContourColor = contourColor;

                // Visa det nya ContourColor-värdet
                Console.WriteLine($"New ContourColor - Type: {threeDFormat.ContourColor.Type}, ARGB: {threeDFormat.ContourColor.Argb}");

                // Spara arbetsboken för att se effekterna
                workbook.Save("ThreeDFormatContourColorDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


