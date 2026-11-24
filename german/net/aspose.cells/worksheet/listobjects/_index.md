---
title: "Worksheet.ListObjects"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt alle ListObjects in diesem Arbeitsblatt zurück"
type: docs
url: /de/net/aspose.cells/worksheet/listobjects/
---
## Worksheet.ListObjects property

Ruft alle ListObjects in diesem Arbeitsblatt ab.

```csharp
public ListObjectCollection ListObjects { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyListObjectsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);
            
            // Erstelle ein ListObject (Tabelle)
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[index];
            table.DisplayName = "ProductTable";
            table.ShowTotals = true;
            
            // Tabellengröße ändern, um mehr Zeilen einzuschließen
            table.Resize(table.StartRow, table.StartColumn, 5, table.EndColumn, true);
            
            // Mehr Daten zur erweiterten Tabelle hinzufügen
            worksheet.Cells["A4"].PutValue("Item3");
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["A5"].PutValue("Item4");
            worksheet.Cells["B5"].PutValue(400);
            
            // Zugriff auf die Tabelle über die ListObjects-Eigenschaft
            ListObject retrievedTable = worksheet.ListObjects["ProductTable"];
            retrievedTable.ShowHeaderRow = true;
            
            // Speichere die Arbeitsmappe
            workbook.Save("ListObjectsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListObjectCollection](../../../aspose.cells.tables/listobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


