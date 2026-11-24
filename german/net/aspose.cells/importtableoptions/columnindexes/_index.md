---
title: "ImportTableOptions.ColumnIndexes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImportTableOptions Eigenschaft. Gibt die 0‑basierten Spalten an, die aus der Datenquelle importiert werden sollen, oder legt sie fest. null bedeutet, dass alle Spalten importiert werden sollen."
type: docs
url: /de/net/aspose.cells/importtableoptions/columnindexes/
---
## ImportTableOptions.ColumnIndexes property

Liest oder legt die Spalten (0-basiert) fest, die aus der Datenquelle importiert werden sollen. Null bedeutet, dass alle Spalten importiert werden.

```csharp
public int[] ColumnIndexes { get; set; }
```

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyColumnIndexesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispiel-DataTable erstellen.
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            
            // Fügen Sie Beispieldaten hinzu
            dataTable.Rows.Add(1, "Product A", 19.99m);
            dataTable.Rows.Add(2, "Product B", 29.99m);
            dataTable.Rows.Add(3, "Product C", 39.99m);

            // Importoptionen so festlegen, dass nur die Spalten mit den Indizes 0 und 2 (ID und Preis) importiert werden
            ImportTableOptions options = new ImportTableOptions();
            options.ColumnIndexes = new int[] { 0, 2 };
            options.IsFieldNameShown = true;

            // Daten mit angegebenen Spaltenindizes importieren
            worksheet.Cells.ImportData(dataTable, 0, 0, options);

            // Speichere die Arbeitsmappe
            workbook.Save("ColumnIndexesDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


