---
title: "ExportTableOptions.IsVertical"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExportTableOptions-Eigenschaft. Wahr, wenn eine Zeile in der Arbeitsmappendatei eine Zeile in der DataTable darstellt. Falsch, wenn eine Spalte in der Arbeitsmappendatei eine Zeile in der DataTable darstellt"
type: docs
url: /de/net/aspose.cells/exporttableoptions/isvertical/
---
## ExportTableOptions.IsVertical property

True, wenn eine Zeile in der Arbeitsmappendatei eine Zeile in der DataTable darstellt. False, wenn eine Spalte in der Arbeitsmappendatei eine Zeile in der DataTable darstellt.

```csharp
public bool IsVertical { get; set; }
```

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyIsVerticalDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Beispieldaten im Arbeitsblatt erstellen
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(25);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(30);

            // DataTable erstellen
            DataTable dt = new DataTable();
            dt.Columns.Add("Column1", typeof(string));
            dt.Columns.Add("Column2", typeof(int));

            // ExportTableOptions mit IsVertical = true festlegen
            ExportTableOptions options = new ExportTableOptions();
            options.IsVertical = true;
            options.ExportColumnName = true;
            options.DataTable = dt;

            // Daten vertikal exportieren
            cells.ExportDataTable(0, 0, 2, 2, options);

            // Exportierte DataTable anzeigen
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row[0]}, {row[1]}");
            }
        }
    }
}
```

### Siehe auch

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


