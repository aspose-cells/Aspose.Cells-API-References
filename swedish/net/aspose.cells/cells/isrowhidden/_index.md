---
title: "Cells.IsRowHidden"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Kontrollerar om en rad på angivet index är dold"
type: docs
url: /sv/net/aspose.cells/cells/isrowhidden/
---
## Cells.IsRowHidden method

Kontrollerar om en rad på angivet index är dold.

```csharp
public bool IsRowHidden(int rowIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | Int32 | radindex |

### Returvärde

true om raden är dold

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsRowHiddenWithInt32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Exempeldata
            cells[1, 0].PutValue("US");
            cells[2, 0].PutValue("UK");
            cells[3, 0].PutValue("India");
            cells[4, 0].PutValue("UK");
            cells[5, 0].PutValue("India");
            cells[6, 0].PutValue("US");
            
            // Applicera filter
            AutoFilter af = sheet.AutoFilter;
            af.Range = "A1:A1";
            af.Filter(0, "India");
            af.Refresh();
            
            // Kontrollera radens synlighet
            Console.WriteLine("Row Visibility Check:");
            for (int i = 1; i < 7; i++)
            {
                Console.WriteLine($"Row {i} hidden: {cells.IsRowHidden(i)}");
            }
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


