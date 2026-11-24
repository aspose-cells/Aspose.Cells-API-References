---
title: "ListColumn.Range"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListColumn-Eigenschaft. Gibt den Bereich dieser ListColumn zurück."
type: docs
url: /de/net/aspose.cells.tables/listcolumn/range/
---
## ListColumn.Range property

Liefert den Bereich dieser Listenspalte.

```csharp
public Range Range { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten hinzufügen, um ein List-Objekt zu erstellen.
            worksheet.Cells["A1"].PutValue("Column1");
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells["A" + i].PutValue("Item " + i);
            }
            
            // Erstelle ein Listenobjekt
            int idx = worksheet.ListObjects.Add(0, 0, 4, 0, true);
            ListObject listObj = worksheet.ListObjects[idx];
            
            // Erhalte die erste ListColumn.
            ListColumn listCol = listObj.ListColumns[0];
            
            // Zugriff auf den Bereich der ListColumn.
            Aspose.Cells.Range range = listCol.Range;
            
            // Bereichsinformationen anzeigen.
            Console.WriteLine("Range address: " + range.Address);
            Console.WriteLine("Row count: " + range.RowCount);
            Console.WriteLine("Column count: " + range.ColumnCount);
            
            // Zellen im Bereich ändern.
            for (int i = 0; i < range.RowCount; i++)
            {
                range[i, 0].PutValue("Modified " + (i + 1));
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("ListColumnRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../../../aspose.cells/range/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


