---
title: "ExportTableOptions.ExportAsString"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExportTableOptions-Eigenschaft. Exportiert den Zeichenkettenwert der Zellen in die DataTable"
type: docs
url: /de/net/aspose.cells/exporttableoptions/exportasstring/
---
## ExportTableOptions.ExportAsString property

Exportiert den Zeichenkettenwert der Zellen in die DataTable.

```csharp
public bool ExportAsString { get; set; }
```

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten mit gemischten Typen hinzufügen
            worksheet.Cells[0, 0].PutValue("ID");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue(1);
            worksheet.Cells[1, 1].PutValue(123.45);
            worksheet.Cells[2, 0].PutValue(2);
            worksheet.Cells[2, 1].PutValue("TextValue");

            // Exportoptionen erstellen mit ExportAsString auf true gesetzt
            ExportTableOptions exportOptions = new ExportTableOptions
            {
                ExportColumnName = true,
                ExportAsString = true // This forces all values to be exported as strings
            };

            // Daten in DataTable exportieren
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 2, exportOptions);

            // Die exportierten Datentypen anzeigen
            Console.WriteLine("Data exported with ExportAsString=true:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row[0]} ({row[0].GetType().Name}) | {row[1]} ({row[1].GetType().Name})");
            }

            // Jetzt exportieren mit ExportAsString=false
            exportOptions.ExportAsString = false;
            DataTable dataTable2 = worksheet.Cells.ExportDataTable(0, 0, 3, 2, exportOptions);

            Console.WriteLine("\nData exported with ExportAsString=false:");
            foreach (DataRow row in dataTable2.Rows)
            {
                Console.WriteLine($"{row[0]} ({row[0].GetType().Name}) | {row[1]} ({row[1].GetType().Name})");
            }
        }
    }
}
```

### Siehe auch

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


