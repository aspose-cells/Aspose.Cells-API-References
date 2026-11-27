---
title: "Cells.Rows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-egenskap. Hämtar samlingen av Row-objekt som representerar de enskilda raderna i detta kalkylblad"
type: docs
url: /sv/net/aspose.cells/cells/rows/
---
## Cells.Rows property

Hämtar samlingen av [`Row`](../../row/) objekt som representerar de enskilda raderna i detta kalkylblad.

```csharp
public RowCollection Rows { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyRowsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange kolumnbredd och radhöjd
            worksheet.Cells.SetColumnWidthPixel(0, 200);
            worksheet.Cells.Rows[0].Height = 50;
            
            // Kom åt radegenskaper via Rows-samlingen
            Row row = worksheet.Cells.Rows[0];
            Console.WriteLine($"Row 0 height: {row.Height}");
            Console.WriteLine($"Is height matched: {row.IsHeightMatched}");
            
            // Modifiera radegenskaper
            row.IsHeightMatched = true;
            row.Height = 60;
            
            // Verifiera ändringar
            Console.WriteLine($"Modified row 0 height: {worksheet.Cells.GetRowHeightPixel(0)}");
            Console.WriteLine($"Is height matched after change: {row.IsHeightMatched}");
            
            // Spara arbetsboken
            workbook.Save("CellsPropertyRowsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [RowCollection](../../rowcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


