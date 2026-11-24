---
title: "Row.FirstDataCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Row-Eigenschaft. Gibt die erste nicht leere Zelle in der Zeile zurück"
type: docs
url: /de/net/aspose.cells/row/firstdatacell/
---
## Row.FirstDataCell property

Gibt die erste nicht leere Zelle in der Zeile zurück.

```csharp
public Cell FirstDataCell { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyFirstDataCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Setze Werte in verschiedene Zellen
            cells["A1"].PutValue("Header");
            cells["B2"].PutValue("FirstData");
            cells["C2"].PutValue("SecondData");
            
            // Hole die erste Datenzelle in Zeile 1 (Index 0)
            Cell firstDataCellRow1 = cells.Rows[0].FirstDataCell;
            Console.WriteLine("First data cell in row 1: " + (firstDataCellRow1 != null ? firstDataCellRow1.Name : "null"));
            
            // Hole die erste Datenzelle in Zeile 2 (Index 1)
            Cell firstDataCellRow2 = cells.Rows[1].FirstDataCell;
            Console.WriteLine("First data cell in row 2: " + firstDataCellRow2.Name);
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


