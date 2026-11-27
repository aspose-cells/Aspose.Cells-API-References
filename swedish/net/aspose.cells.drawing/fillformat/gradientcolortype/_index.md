---
title: "FillFormat.GradientColorType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FillFormat-egenskap. Returnerar gradientfärgstypen för den specificerade fyllningen"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/gradientcolortype/
---
## FillFormat.GradientColorType property

Returnerar gradientfärgens typ för den angivna fyllningen.

```csharp
public GradientColorType GradientColorType { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class FillFormatPropertyGradientColorTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form för att demonstrera gradientfyllning
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            try
            {
                // Ställ in en tvåfärgsgradientfyllning
                shape.Fill.SetTwoColorGradient(Color.Red, Color.Blue,
                    GradientStyleType.Horizontal, 2);

                // Åtkomst till FillFormat för att hämta GradientColorType
                FillFormat fillFormat = shape.Fill;

                // Visa GradientColorType-värdet
                Console.WriteLine("GradientColorType: " + fillFormat.GradientColorType);

                // Spara arbetsboken
                workbook.Save("GradientColorTypeDemo.xlsx");
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

* enum [GradientColorType](../../gradientcolortype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


