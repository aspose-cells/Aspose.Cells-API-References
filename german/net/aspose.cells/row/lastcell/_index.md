---
title: "Row.LastCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Row‑Eigenschaft. Gibt das letzte Zellenobjekt in der Zeile zurück."
type: docs
url: /de/net/aspose.cells/row/lastcell/
---
## Row.LastCell property

Gibt das letzte Zellenobjekt in der Zeile zurück.

```csharp
public Cell LastCell { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyLastCellDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("First");
            worksheet.Cells["B1"].PutValue("Second");
            worksheet.Cells["C1"].PutValue("Last");

            // Rufen Sie die erste Zeile ab
            Row row = worksheet.Cells.Rows[0];

            // Greifen Sie auf die letzte Zelle in der Zeile zu
            Cell lastCell = row.LastCell;
            
            // Geben Sie den Wert der letzten Zelle aus
            Console.WriteLine("Last cell value: " + lastCell.Value);
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


