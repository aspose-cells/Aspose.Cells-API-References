---
title: "ExportTableOptions.PlotVisibleRows"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExportTableOptions-Eigenschaft. Exportiert nur sichtbare Zeilen"
type: docs
url: /de/net/aspose.cells/exporttableoptions/plotvisiblerows/
---
## ExportTableOptions.PlotVisibleRows property

Exportiert nur sichtbare Zeilen.

```csharp
public bool PlotVisibleRows { get; set; }
```

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyPlotVisibleRowsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe und greifen Sie auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Beispieldaten im Arbeitsblatt erstellen
            cells["A1"].PutValue("Column1");
            cells["A2"].PutValue(10);
            cells["A3"].PutValue(20);
            cells["A4"].PutValue(30);

            // Zeile 3 ausblenden (Index 2), die den Wert 20 enthält
            worksheet.Cells.HideRow(2);

            // Erstelle eine DataTable, zu der exportiert werden soll
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Column1", typeof(int));

            // Exportoptionen einrichten
            ExportTableOptions options = new ExportTableOptions();
            options.PlotVisibleRows = true; // Only export visible rows
            options.ExportColumnName = true;
            options.DataTable = dataTable;

            // Daten exportieren (sollte ausgeblendete Zeile überspringen)
            cells.ExportDataTable(0, 0, 4, 1, options);

            // Zeige die exportierten Daten an
            Console.WriteLine("Exported Data (PlotVisibleRows=true):");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine(row["Column1"]);
            }
        }
    }
}
```

### Siehe auch

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


