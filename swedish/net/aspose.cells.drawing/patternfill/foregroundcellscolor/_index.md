---
title: "PatternFill.ForegroundCellsColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PatternFill-egenskap. Hämtar och anger förgrundens CellsColor-objekt"
type: docs
url: /sv/net/aspose.cells.drawing/patternfill/foregroundcellscolor/
---
## PatternFill.ForegroundCellsColor property

Hämtar och anger förgrundens [`CellsColor`](../../../aspose.cells/cellscolor/) objekt.

```csharp
public CellsColor ForegroundCellsColor { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class PatternFillPropertyForegroundCellsColorDemo
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

                // Skapa ett CellsColor-objekt för förgrunden med Color-egenskapen
                // Eftersom CellsColor inte har en publik konstruktor, kommer vi att använda den befintliga ForegroundCellsColor
                // och ändra dess egenskaper direkt
                patternFill.ForegroundCellsColor.Color = Color.Blue;
                patternFill.ForegroundCellsColor.Argb = Color.Blue.ToArgb();

                // Visa egenskaperna för ForegroundCellsColor
                Console.WriteLine("ForegroundCellsColor Type: " + patternFill.ForegroundCellsColor.Type);
                Console.WriteLine("ForegroundCellsColor Color: " + patternFill.ForegroundCellsColor.Color);
                Console.WriteLine("ForegroundCellsColor ARGB: " + patternFill.ForegroundCellsColor.Argb);

                // Spara arbetsboken
                workbook.Save("ForegroundCellsColorDemo.xlsx");
                Console.WriteLine("ForegroundCellsColor demonstration completed successfully.");
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


