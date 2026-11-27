---
title: "CellsColor-egenskap. Hämtar och anger färgindexet i färgpaletten. Gäller endast för indexerade färger"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Definiera ett område som vi ska applicera en färgad kant på"
type: docs
url: /sv/net/aspose.cells/cellscolor/colorindex/
---
## CellsColor.ColorIndex property

Hämtar och sätter färgindexet i färgpaletten. Gäller endast för indexerad färg.

```csharp
public int ColorIndex { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;

    public class CellsColorPropertyColorIndexDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ange ColorIndex (palettindex) – till exempel 5
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:D4");

            // Skapa en CellsColor-instans
            CellsColor cellsColor = workbook.CreateCellsColor();

            // Applicera CellsColor som den inre kantfärgen för området
            cellsColor.ColorIndex = 5;

            // Läs och visa det aktuella ColorIndex‑värdet
            range.SetInsideBorders(BorderType.Horizontal | BorderType.Vertical,
                                   CellBorderType.Thin,
                                   cellsColor);

            // CellsColor.Color
            Console.WriteLine("Current ColorIndex value: " + cellsColor.ColorIndex);

            // Spara arbetsboken för att visualisera resultatet
            try
            {
                workbook.Save("ColorIndexDemo.xlsx");
                Console.WriteLine("Workbook saved as ColorIndexDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


