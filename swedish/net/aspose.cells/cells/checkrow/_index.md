---
title: "Cells.CheckRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Hämtar Row-elementet eller null på det angivna cellradindexet"
type: docs
url: /sv/net/aspose.cells/cells/checkrow/
---
## Cells.CheckRow method

Hämtar [`Row`](../../row/) elementet eller null på det angivna cellradindexet.

```csharp
public Row CheckRow(int row)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex |

### Returvärde

Returnerar [`Row`](../../row/) objektet om radobjektet finns, annars returneras null.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckRowWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Fyll i lite data
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(100);
            cells["A3"].PutValue(200);
            
            // Kontrollera om raden finns och hämta radobjektet
            Row row = cells.CheckRow(1);
            if (row != null)
            {
                Console.WriteLine("Row 1 exists with height: " + row.Height);
            }
            
            // Kontrollera icke-existerande rad
            Row nonExistentRow = cells.CheckRow(100);
            Console.WriteLine("Row 100 exists: " + (nonExistentRow != null));
        }
    }
}
```

### Se även

* class [Row](../../row/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


