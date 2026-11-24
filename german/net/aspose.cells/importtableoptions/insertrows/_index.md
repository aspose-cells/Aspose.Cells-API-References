---
title: "ImportTableOptions.InsertRows"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImportTableOptions Eigenschaft. Gibt an, ob neue Zeilen für das Importieren von Daten­datensätzen hinzugefügt werden sollen"
type: docs
url: /de/net/aspose.cells/importtableoptions/insertrows/
---
## ImportTableOptions.InsertRows property

Gibt an, ob neue Zeilen für das Importieren von Datensätzen hinzugefügt werden sollen.

```csharp
public bool InsertRows { get; set; }
```

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyInsertRowsDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Beispieltabelle erstellen
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            dataTable.Rows.Add(1, "Laptop", 999.99);
            dataTable.Rows.Add(2, "Monitor", 249.99);
            dataTable.Rows.Add(3, "Keyboard", 49.99);

            // Vorhandene Daten zum Arbeitsblatt hinzufügen (werden durch Einfügen nach unten verschoben)
            cells["A1"].PutValue("Existing Data");
            cells["A2"].PutValue(100);

            // Importoptionen mit InsertRows = true festlegen
            ImportTableOptions options = new ImportTableOptions();
            options.InsertRows = true; // This will insert new rows instead of overwriting
            options.IsFieldNameShown = true;

            // Daten ab Zeile 1 importieren (fügt Zeilen unterhalb der vorhandenen Daten ein)
            cells.ImportData(dataTable, 1, 0, options);

            // Speichere die Arbeitsmappe
            workbook.Save("InsertRowsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


