---
title: "Row.LastDataCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Row-Eigenschaft. Gibt die letzte nicht leere Zelle in der Zeile zurück"
type: docs
url: /de/net/aspose.cells/row/lastdatacell/
---
## Row.LastDataCell property

Gibt die letzte nicht leere Zelle in der Zeile zurück.

```csharp
public Cell LastDataCell { get; }
```

### Beispiele

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
            
            // Daten in Zellen einfügen
            cells["A1"].PutValue("First cell");
            cells["B1"].PutValue("Second cell");
            cells["C2"].PutValue("Not in first row");
            
            // Letzte Datenzelle in der ersten Zeile abrufen
            Cell lastDataCell = cells.Rows[0].LastDataCell;
            
            Console.WriteLine("Last data cell in first row: " + lastDataCell.Name);
            Console.WriteLine("Value in last data cell: " + lastDataCell.StringValue);
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


