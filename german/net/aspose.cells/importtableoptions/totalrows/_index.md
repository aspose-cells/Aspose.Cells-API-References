---
title: "ImportTableOptions.TotalRows"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImportTableOptions-Eigenschaft. Gibt die Gesamtzahl der Zeilen an, die aus der Datenquelle importiert werden sollen, oder legt sie fest. 1 bedeutet alle Zeilen der angegebenen Datenquelle"
type: docs
url: /de/net/aspose.cells/importtableoptions/totalrows/
---
## ImportTableOptions.TotalRows property

Liest oder legt die Gesamtanzahl der zu importierenden Zeilen aus der Datenquelle fest. -1 bedeutet, dass alle Zeilen der angegebenen Datenquelle importiert werden.

```csharp
public int TotalRows { get; set; }
```

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyTotalRowsDemo
    {
        public static void Run()
        {
            // Erstelle ein Beispiel-DataTable
            DataTable table = new DataTable("TestTable");
            table.Columns.Add("Column1", typeof(string));
            table.Columns.Add("Column2", typeof(int));
            
            // Fügen Sie Beispieldaten hinzu
            table.Rows.Add("Item1", 100);
            table.Rows.Add("Item2", 200);
            table.Rows.Add("Item3", 300);

            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle ImportTableOptions mit TotalRows auf 2 gesetzt (es werden nur die ersten 2 Zeilen importiert)
            ImportTableOptions options = new ImportTableOptions
            {
                IsFieldNameShown = true,
                TotalRows = 2 // Only import 2 rows from the DataTable
            };

            // Importiere Daten mit den angegebenen Optionen
            worksheet.Cells.ImportData(table, 0, 0, options);

            // Speichere die Arbeitsmappe
            workbook.Save("ImportWithTotalRows.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Data imported with TotalRows=2. Only first 2 rows were imported.");
        }
    }
}
```

### Siehe auch

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


