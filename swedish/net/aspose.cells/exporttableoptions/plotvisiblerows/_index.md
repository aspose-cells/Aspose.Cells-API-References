---
title: "ExportTableOptions.PlotVisibleRows"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExportTableOptions egenskap. Exporterar endast synliga rader"
type: docs
url: /sv/net/aspose.cells/exporttableoptions/plotvisiblerows/
---
## ExportTableOptions.PlotVisibleRows property

Exporterar endast synliga rader.

```csharp
public bool PlotVisibleRows { get; set; }
```

### Exempel

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
            // Skapa en arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa exempeldata i kalkylbladet
            cells["A1"].PutValue("Column1");
            cells["A2"].PutValue(10);
            cells["A3"].PutValue(20);
            cells["A4"].PutValue(30);

            // Dölj rad 3 (index 2) som innehåller värdet 20
            worksheet.Cells.HideRow(2);

            // Skapa en DataTable att exportera till
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Column1", typeof(int));

            // Ställ in exportalternativ
            ExportTableOptions options = new ExportTableOptions();
            options.PlotVisibleRows = true; // Only export visible rows
            options.ExportColumnName = true;
            options.DataTable = dataTable;

            // Exportera data (bör hoppa över dold rad)
            cells.ExportDataTable(0, 0, 4, 1, options);

            // Visa den exporterade datan
            Console.WriteLine("Exported Data (PlotVisibleRows=true):");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine(row["Column1"]);
            }
        }
    }
}
```

### Se även

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


