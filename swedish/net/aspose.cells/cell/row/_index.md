---
title: "Cell.Row"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-egenskap. Hämtar radnummer nollbaserat för cellen"
type: docs
url: /sv/net/aspose.cells/cell/row/
---
## Cell.Row property

Hämtar radnumret (nollbaserat) för cellen.

```csharp
public int Row { get; }
```

### Property Value

Cellradnummer

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyRowDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata och formel
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");
            
            // Hitta cell som innehåller formel
            Cell cell = worksheet.Cells.Find("=SUM(A1", null, new FindOptions()
            { 
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains 
            });
            
            // Demonstrera Row-egenskapen
            Console.WriteLine("Formula found in row: " + cell.Row);
            Console.WriteLine("Formula found in column: " + cell.Column);
            
            // Verifiera att raden är korrekt
            if (cell.Row == 2 && cell.Column == 0)
            {
                Console.WriteLine("Row property works correctly");
            }
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


