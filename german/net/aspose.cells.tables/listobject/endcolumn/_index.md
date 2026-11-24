---
title: "ListObject.EndColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListObject-Eigenschaft. Gibt die Endspalte des Bereichs zurück"
type: docs
url: /de/net/aspose.cells.tables/listobject/endcolumn/
---
## ListObject.EndColumn property

Liest die Endspalte des Bereichs.

```csharp
public int EndColumn { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyEndColumnDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Age");
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue(i-1);
                worksheet.Cells[$"B{i}"].PutValue($"Person {i-1}");
                worksheet.Cells[$"C{i}"].PutValue(20 + i);
            }

            // Ein Listenobjekt/Tabelle erstellen
            int listObjectIndex = worksheet.ListObjects.Add(0, 0, 4, 2, true);
            ListObject table = worksheet.ListObjects[listObjectIndex];
            table.ShowTotals = true;
            
            // Ursprüngliche Endspalte anzeigen
            Console.WriteLine($"Original EndColumn: {table.EndColumn}");
            
            // Tabellengröße ändern, um eine weitere Spalte hinzuzufügen
            table.Resize(table.StartRow, table.StartColumn, table.EndRow, table.EndColumn + 1, table.ShowHeaderRow);
            
            // Neue Endspalte anzeigen
            Console.WriteLine($"New EndColumn: {table.EndColumn}");
            
            // Speichere die Arbeitsmappe
            workbook.Save("ListObjectEndColumnDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


