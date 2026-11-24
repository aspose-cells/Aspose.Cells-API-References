---
title: "ListObject.EndRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListObject-Eigenschaft. Gibt die Endzeile des Bereichs zurück"
type: docs
url: /de/net/aspose.cells.tables/listobject/endrow/
---
## ListObject.EndRow property

Liest die Endzeile des Bereichs.

```csharp
public int EndRow { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyEndRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Erstelle Beispieldaten
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["A3"].PutValue("Mary");
            sheet.Cells["B3"].PutValue(25);
            
            // ListObject/Tabelle erstellen
            int idx = sheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = sheet.ListObjects[idx];
            
            // Initialen EndRow anzeigen
            Console.WriteLine("Initial EndRow: " + table.EndRow);
            
            // Neue Zeile zur Tabelle hinzufügen
            table.PutCellValue(4, 0, "Tom");
            table.PutCellValue(4, 1, 28);
            
            // Aktualisierten EndRow anzeigen
            Console.WriteLine("Updated EndRow: " + table.EndRow);
            
            // Speichere die Arbeitsmappe
            wb.Save("ListObjectEndRowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


