---
title: "ImportTableOptions.IsFieldNameShown"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImportTableOptions-Eigenschaft. Gibt an, ob der Feldname importiert werden soll"
type: docs
url: /de/net/aspose.cells/importtableoptions/isfieldnameshown/
---
## ImportTableOptions.IsFieldNameShown property

Gibt an, ob Feldnamen importiert werden sollen.

```csharp
public bool IsFieldNameShown { get; set; }
```

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyIsFieldNameShownDemo
    {
        public static void Run()
        {
            // Erstelle ein Beispiel-DataTable
            DataTable table = new DataTable();
            table.Columns.Add("ID");
            table.Columns.Add("Product");
            
            // Fügen Sie Beispieldaten hinzu
            table.Rows.Add(1, "Laptop");
            table.Rows.Add(2, "Smartphone");
            table.Rows.Add(3, "Tablet");

            // Erstelle eine Arbeitsmappe und importiere Daten mit angezeigten Feldnamen
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;  // Show field names
            options.InsertRows = true;       // Insert new rows
            
            // Importiere Daten beginnend ab Zeile 5, Spalte 0
            cells.ImportData(table, 5, 0, options);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ImportDataWithFieldNames.xlsx");
        }
    }
}
```

### Siehe auch

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


