---
title: "Enum FormatSetType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.FormatSetType enum. Typ för fyllningsformat."
type: docs
url: /sv/net/aspose.cells.drawing/formatsettype/
---
## FormatSetType enumeration

Fyllningsformatuppsättningstyp.

```csharp
public enum FormatSetType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `0` | Ingen fyllning. |
| IsGradientSet | `1` | Gradientfyllningsformat. |
| IsTextureSet | `2` | Texturfyllningsformat. |
| IsPatternSet | `3` | Mönsterfyllningsformat. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassFormatSetTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till en form för att demonstrera fyllningsformatet
                Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 200);
                FillFormat fillFormat = shape.Fill;

                // Visa initial fyllningstyp
                Console.WriteLine("Initial fill type: " + fillFormat.Type);

                // Demonstrera FormatSetType enum-värden
                Console.WriteLine("FormatSetType.None: " + (int)FormatSetType.None);
                Console.WriteLine("FormatSetType.IsGradientSet: " + (int)FormatSetType.IsGradientSet);
                Console.WriteLine("FormatSetType.IsTextureSet: " + (int)FormatSetType.IsTextureSet);
                Console.WriteLine("FormatSetType.IsPatternSet: " + (int)FormatSetType.IsPatternSet);

                // Applicera olika fyllningstyper med FormatSetType
                fillFormat.Type = (FillType)FormatSetType.IsGradientSet;
                Console.WriteLine("After setting gradient: " + fillFormat.Type);

                fillFormat.Type = (FillType)FormatSetType.IsPatternSet;
                Console.WriteLine("After setting pattern: " + fillFormat.Type);

                // Spara arbetsboken
                workbook.Save("FormatSetTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with FormatSetType: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


