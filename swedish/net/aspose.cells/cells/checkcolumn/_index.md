---
title: "Cells.CheckColumn"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar Column-elementet eller null på det angivna kolumnindexet"
type: docs
url: /sv/net/aspose.cells/cells/checkcolumn/
---
## Cells.CheckColumn method

Hämtar [`Column`](../../column/)-elementet eller null på det angivna kolumnindexet.

```csharp
public Column CheckColumn(int columnIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | Int32 | Kolumnindexet. |

### Returvärde

Column-objektet.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckColumnWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Ange ett värde i kolumn 1 (B3)
            cells["B3"].PutValue("Sample Data");
            
            // Kontrollera kolumn 4 (E-kolumnen)
            Column column = cells.CheckColumn(4);
            
            // Skriv ut kolumnegenskaper
            Console.WriteLine("Column Width: " + column.Width);
            Console.WriteLine("Column Index: " + column.Index);
        }
    }
}
```

### Se även

* class [Column](../../column/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


