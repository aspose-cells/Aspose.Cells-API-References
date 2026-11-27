---
title: "Row.LastDataCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Row-egenskap. Hämtar den sista icke-tomma cellen i raden"
type: docs
url: /sv/net/aspose.cells/row/lastdatacell/
---
## Row.LastDataCell property

Hämtar den sista icke‑tomma cellen i raden.

```csharp
public Cell LastDataCell { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyLastDataCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Sätt in data i celler
            cells["A1"].PutValue("First cell");
            cells["B1"].PutValue("Second cell");
            cells["C2"].PutValue("Not in first row");
            
            // Hämta sista datacellen i första raden
            Cell lastDataCell = cells.Rows[0].LastDataCell;
            
            Console.WriteLine("Last data cell in first row: " + lastDataCell.Name);
            Console.WriteLine("Value in last data cell: " + lastDataCell.StringValue);
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


