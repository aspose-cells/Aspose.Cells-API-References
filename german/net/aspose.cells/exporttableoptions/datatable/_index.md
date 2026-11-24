---
title: "ExportTableOptions.DataTable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExportTableOptions-Eigenschaft. Liest und setzt die DataTable, der die Spaltendatentypen zugewiesen sind"
type: docs
url: /de/net/aspose.cells/exporttableoptions/datatable/
---
## ExportTableOptions.DataTable property

Liest und setzt die DataTable, deren Spalten-Datentyp zugewiesen ist.

```csharp
public DataTable DataTable { get; set; }
```

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyDataTableDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Füge Beispieldaten zu Zellen hinzu
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue(100);
            cells["B2"].PutValue("Text1");
            cells["A3"].PutValue(200);
            cells["B3"].PutValue("Text2");

            // DataTable erstellen und Spalten definieren
            DataTable dt = new DataTable();
            dt.Columns.Add("NumericData", typeof(double));
            dt.Columns.Add("TextData", typeof(string));

            // Exportoptionen konfigurieren
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true;
            options.Indexes = new int[] { 0, 1 }; // Export both columns
            options.DataTable = dt;

            // Daten in DataTable exportieren
            cells.ExportDataTable(0, 0, 3, 2, options);

            // Exportierte Daten anzeigen
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row["NumericData"]}, {row["TextData"]}");
            }
        }
    }
}
```

### Siehe auch

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


