---
title: "ExportTableOptions.ExportColumnName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExportTableOptions‑Eigenschaft. Gibt an, ob die Daten in der ersten Zeile zum Spaltennamen der DataTable exportiert werden. Der Standardwert ist false."
type: docs
url: /de/net/aspose.cells/exporttableoptions/exportcolumnname/
---
## ExportTableOptions.ExportColumnName property

Gibt an, ob die Daten in der ersten Zeile in den Spaltennamen der DataTable exportiert werden. Der Standardwert ist false.

```csharp
public bool ExportColumnName { get; set; }
```

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyExportColumnNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Beispieldaten im Arbeitsblatt erstellen
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue(100);
            cells["B2"].PutValue("Data1");
            cells["A3"].PutValue(200);
            cells["B3"].PutValue("Data2");

            // Exportoptionen konfigurieren
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true; // Demonstrating ExportColumnName property
            options.IsVertical = true;
            options.Indexes = new int[] { 0, 1 }; // Export all columns

            // Daten vom Arbeitsblatt in die DataTable exportieren
            DataTable dataTable = cells.ExportDataTable(0, 0, 4, 2, options);

            // Exportierte Daten anzeigen
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row["Column1"]}, {row["Column2"]}");
            }
        }
    }
}
```

### Siehe auch

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


