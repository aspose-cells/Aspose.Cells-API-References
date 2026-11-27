---
title: "PatternFill.ForeTransparency"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PatternFill-egenskap. Hämtar eller anger genomskinligheten för förgrundsfärgen"
type: docs
url: /sv/net/aspose.cells.drawing/patternfill/foretransparency/
---
## PatternFill.ForeTransparency property

Hämtar eller anger transparensen för förgrundsfärgen.

```csharp
public double ForeTransparency { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyForeTransparencyDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform för att demonstrera mönsterfyllning
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            // Ställ in fyllningstyp till mönster
            shape.Fill.FillType = FillType.Pattern;

            // Hämta PatternFill-instansen
            PatternFill patternFill = shape.Fill.PatternFill;

            // Konfigurera PatternFill-egenskaper
            patternFill.Pattern = FillPattern.Solid;
            patternFill.ForegroundColor = Color.Red;
            patternFill.BackgroundColor = Color.Blue;

            try
            {
                // Visa det ursprungliga värdet för ForeTransparency
                Console.WriteLine("Initial ForeTransparency value: " + patternFill.ForeTransparency);

                // Ange ett nytt värde för ForeTransparency (50 % genomskinlighet)
                patternFill.ForeTransparency = 0.5;

                // Visa det uppdaterade värdet för ForeTransparency
                Console.WriteLine("Updated ForeTransparency value: " + patternFill.ForeTransparency);

                // Spara arbetsboken
                workbook.Save("ForeTransparencyDemo.xlsx");
                Console.WriteLine("ForeTransparency demonstration completed successfully.");
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

* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


