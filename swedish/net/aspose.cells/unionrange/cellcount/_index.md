---
title: "UnionRange.CellCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "UnionRange‑egenskap. Hämtar antalet celler i området"
type: docs
url: /sv/net/aspose.cells/unionrange/cellcount/
---
## UnionRange.CellCount property

Hämtar antalet celler i området.

```csharp
public int CellCount { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyCellCountDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i data i kalkylbladet
            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].Value = $"Cell {row + 1},{col + 1}";
                }
            }

            // Skapa områden och kombinera dem till ett unionområde
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B3");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("D1:E4");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // Visa egenskapen CellCount
            Console.WriteLine("Total cells in union range: " + unionRange.CellCount);

            // Beräkna förväntat antal celler
            int expectedCount = (range1.RowCount * range1.ColumnCount) + (range2.RowCount * range2.ColumnCount);
            Console.WriteLine("Expected cell count: " + expectedCount);

            // Visa användning genom att iterera genom celler
            Console.WriteLine("\nCell values in the union range:");
            int cellCounter = 0;
            foreach (Cell cell in unionRange)
            {
                Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                cellCounter++;
            }

            // Verifiera att antalet celler matchar iterationen
            Console.WriteLine($"\nIterated through {cellCounter} cells (should match CellCount)");

            // Skapa ett annat unionområde med olika dimensioner
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("A5:E5");
            Aspose.Cells.Range range4 = worksheet.Cells.CreateRange("C1:C5");
            UnionRange unionRange2 = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range3, range4 });

            // Jämför cellantal för olika unionområden
            Console.WriteLine("\nSecond union range cell count: " + unionRange2.CellCount);
            Console.WriteLine("First union range has " + 
                (unionRange.CellCount > unionRange2.CellCount ? "more" : "fewer") + 
                " cells than second union range");

            // Spara arbetsboken
            workbook.Save("UnionRangeCellCountDemo.xlsx");
        }
    }
}
```

### Se även

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


