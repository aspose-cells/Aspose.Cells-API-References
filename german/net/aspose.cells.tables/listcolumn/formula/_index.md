---
title: "ListColumn.Formula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListColumn-Eigenschaft. Gibt die Formel der ListColumn zurück und legt sie fest."
type: docs
url: /de/net/aspose.cells.tables/listcolumn/formula/
---
## ListColumn.Formula property

Liefert und setzt die Formel der Listenspalte.

```csharp
public string Formula { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnPropertyFormulaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Erstellen Sie Beispieldaten und eine Tabelle
            sheet.Cells["A1"].PutValue("Numbers");
            sheet.Cells["A2"].PutValue(5);
            sheet.Cells["A3"].PutValue(10);
            sheet.Cells["A4"].PutValue(15);
            
            sheet.Cells["B1"].PutValue("Doubled");
            sheet.Cells["B2"].PutValue("=A2*2");
            
            int tableIndex = sheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = sheet.ListObjects[tableIndex];
            table.ShowTotals = true;
            
            // Formel zur ListColumn hinzufügen.
            ListColumn column = table.ListColumns[0];
            column.Formula = "=A2*3"; // This will apply to all cells in the column
            
            // Speichere die Arbeitsmappe
            workbook.Save("ListColumnFormulaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


