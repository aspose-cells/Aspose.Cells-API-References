---
title: "PatternFill.BackgroundCellsColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PatternFill-egenskap. Hämtar och anger förgrundens CellsColor-objekt"
type: docs
url: /sv/net/aspose.cells.drawing/patternfill/backgroundcellscolor/
---
## PatternFill.BackgroundCellsColor property

Hämtar och anger förgrundens [`CellsColor`](../../../aspose.cells/cellscolor/) objekt.

```csharp
public CellsColor BackgroundCellsColor { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyBackgroundCellsColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform för att demonstrera mönsterfyllning
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 100);

            try
            {
                // Ställ in fyllningstyp till mönster
                shape.Fill.FillType = FillType.Pattern;

                // Hämta PatternFill-instansen
                PatternFill patternFill = shape.Fill.PatternFill;

                // Ställ in mönstertyp och färger
                patternFill.Pattern = FillPattern.WideDownwardDiagonal;
                patternFill.ForegroundColor = Color.Red;
                patternFill.BackgroundColor = Color.Yellow;

                // Åtkomst till och ändring av BackgroundCellsColor-egenskaper
                patternFill.BackgroundCellsColor.Color = Color.Blue;
                patternFill.BackgroundCellsColor.Argb = Color.Blue.ToArgb();
                patternFill.BackgroundCellsColor.Transparency = 0.3;

                // Visa egenskaperna för BackgroundCellsColor
                Console.WriteLine("BackgroundCellsColor Type: " + patternFill.BackgroundCellsColor.Type);
                Console.WriteLine("BackgroundCellsColor Color: " + patternFill.BackgroundCellsColor.Color);
                Console.WriteLine("BackgroundCellsColor ARGB: " + patternFill.BackgroundCellsColor.Argb);
                Console.WriteLine("BackgroundCellsColor Transparency: " + patternFill.BackgroundCellsColor.Transparency);

                // Spara arbetsboken
                workbook.Save("BackgroundCellsColorDemo.xlsx");
                Console.WriteLine("BackgroundCellsColor demonstration completed successfully.");
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
* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


