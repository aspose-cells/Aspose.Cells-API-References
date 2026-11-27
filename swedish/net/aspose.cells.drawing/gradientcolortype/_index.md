---
title: "Enum GradientColorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.GradientColorType enum. Representerar gradientfärgstypen för den angivna fyllningen"
type: docs
url: /sv/net/aspose.cells.drawing/gradientcolortype/
---
## GradientColorType enumeration

Representerar gradientfärgstypen för den angivna fyllningen.

```csharp
public enum GradientColorType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ingen gradientfärg |
| OneColor | `1` | En gradientfärg |
| PresetColors | `2` | Förinställda gradientfärger |
| TwoColors | `3` | Två gradientfärger |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassGradientColorTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till en form för att demonstrera gradientfyllning
                Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 200, 200);
                FillFormat fill = shape.Fill;

                // Ställ in gradientfyllningstyp
                fill.FillType = FillType.Gradient;

                // Demonstrera olika värden för GradientColorType enum
                Console.WriteLine("Available GradientColorType values:");
                Console.WriteLine("None: " + GradientColorType.None);
                Console.WriteLine("OneColor: " + GradientColorType.OneColor);
                Console.WriteLine("PresetColors: " + GradientColorType.PresetColors);
                Console.WriteLine("TwoColors: " + GradientColorType.TwoColors);

                // Läs och visa den aktuella gradientfärgtypen (egenskapen är skrivskyddad)
                Console.WriteLine("Current gradient color type: " + fill.GradientColorType);

                // Spara arbetsboken
                workbook.Save("GradientColorTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GradientColorType: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


