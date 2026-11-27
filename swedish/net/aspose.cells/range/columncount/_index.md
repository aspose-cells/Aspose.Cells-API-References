---
title: "Range.ColumnCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range‑egenskap. Hämtar antalet kolumner i området"
type: docs
url: /sv/net/aspose.cells/range/columncount/
---
## Range.ColumnCount property

Hämtar antalet kolumner i området.

```csharp
public int ColumnCount { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyColumnCountDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Skapa exempeldata (5 kolumner x 3 rader)
            for (int col = 0; col < 5; col++)
            {
                for (int row = 0; row < 3; row++)
                {
                    sheet.Cells[row, col].PutValue($"Data {row},{col}");
                }
            }
            
            // Skapa ett område som täcker alla datakolumner
            Aspose.Cells.Range dataRange = sheet.Cells.CreateRange(0, 0, 3, 5);
            
            // Demonstrera användning av ColumnCount
            Console.WriteLine($"Range has {dataRange.ColumnCount} columns");
            
            // Anpassa automatiskt varje kolumn i området
            for (int i = 0; i < dataRange.ColumnCount; i++)
            {
                sheet.AutoFitColumn(dataRange.FirstColumn + i);
            }
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


