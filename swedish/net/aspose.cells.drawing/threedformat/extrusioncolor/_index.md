---
title: "ThreeDFormat.ExtrusionColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreeDFormat-egenskap. Hämtar extruderingsfärgen på en form"
type: docs
url: /sv/net/aspose.cells.drawing/threedformat/extrusioncolor/
---
## ThreeDFormat.ExtrusionColor property

Hämtar extruderingsfärgen på en form.

```csharp
public CellsColor ExtrusionColor { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ThreeDFormatPropertyExtrusionColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera 3D-formatering
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 100);
            shape.Text = "3D ExtrusionColor Demo";
            
            // Hämta ThreeDFormat för formen
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Konfigurera grundläggande 3D-egenskaper för att göra extruderingen synlig
            threeDFormat.ExtrusionHeight = 20;
            threeDFormat.ContourWidth = 2;
            threeDFormat.Material = PresetMaterialType.Plastic;

            try
            {
                // Hämta och visa värdet för ExtrusionColor
                CellsColor extrusionColor = threeDFormat.ExtrusionColor;
                Console.WriteLine("ExtrusionColor properties:");
                Console.WriteLine($"Type: {extrusionColor.Type}");
                Console.WriteLine($"Color (RGB): {extrusionColor.Color}");
                Console.WriteLine($"Transparency: {extrusionColor.Transparency}");

                // Spara arbetsboken för att se 3D-effekterna
                workbook.Save("ThreeDFormatExtrusionColorDemo.xlsx");
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


