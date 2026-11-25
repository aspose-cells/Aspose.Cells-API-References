---
title: "ExportTableOptions.PlotVisibleRows"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExportTableOptions. Esporta solo le righe visibili"
type: docs
url: /it/net/aspose.cells/exporttableoptions/plotvisiblerows/
---
## ExportTableOptions.PlotVisibleRows property

Esporta solo le righe visibili.

```csharp
public bool PlotVisibleRows { get; set; }
```

### Esempi

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
            // Crea una cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Crea dati di esempio nel foglio di lavoro
            cells["A1"].PutValue("Column1");
            cells["A2"].PutValue(10);
            cells["A3"].PutValue(20);
            cells["A4"].PutValue(30);

            // Nascondi la riga 3 (indice 2) che contiene il valore 20
            worksheet.Cells.HideRow(2);

            // Crea un DataTable su cui esportare
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Column1", typeof(int));

            // Configura le opzioni di esportazione
            ExportTableOptions options = new ExportTableOptions();
            options.PlotVisibleRows = true; // Only export visible rows
            options.ExportColumnName = true;
            options.DataTable = dataTable;

            // Esporta i dati (dovrebbe saltare la riga nascosta)
            cells.ExportDataTable(0, 0, 4, 1, options);

            // Visualizza i dati esportati
            Console.WriteLine("Exported Data (PlotVisibleRows=true):");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine(row["Column1"]);
            }
        }
    }
}
```

### Vedi anche

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


