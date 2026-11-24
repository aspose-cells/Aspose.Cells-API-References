---
title: "ListColumn.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListColumn-Eigenschaft. Gibt den Namen der Spalte zurück und legt ihn fest."
type: docs
url: /de/net/aspose.cells.tables/listcolumn/name/
---
## ListColumn.Name property

Liefert und setzt den Namen der Spalte.

```csharp
public string Name { get; set; }
```

### Hinweise

Wenn der Name der Spalte gesetzt wird, ändert sich auch der entsprechende Zellenwert.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle Beispieldaten
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Value");
            
            // Ein Tabellen-/Listenobjekt erstellen
            int index = worksheet.ListObjects.Add(0, 0, 2, 2, true);
            Aspose.Cells.Tables.ListObject listObject = worksheet.ListObjects[index];

            // Zugriff auf und Ändern der Name‑Eigenschaft der ersten ListColumn
            listObject.ListColumns[0].Name = "NewID";
            
            // Überprüfe, ob der Name gesetzt wurde
            Console.WriteLine("First column name: " + listObject.ListColumns[0].Name);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ListColumnPropertyNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


