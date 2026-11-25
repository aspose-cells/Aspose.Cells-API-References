---
title: "ExportTableOptions.PlotVisibleCells"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExportTableOptions. Esporta solo le celle visibili"
type: docs
url: /it/net/aspose.cells/exporttableoptions/plotvisiblecells/
---
## ExportTableOptions.PlotVisibleCells property

Esporta solo le celle visibili.

```csharp
public bool PlotVisibleCells { get; set; }
```

### Esempi

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyPlotVisibleCellsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio con alcune righe/colonne nascoste
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["C1"].PutValue("Header3");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue("Data3");
            
            // Nascondi la riga 2 e la colonna B (indice 1)
            worksheet.Cells.HideRow(1);
            worksheet.Cells.HideColumn(1);

            // Crea le opzioni di esportazione con PlotVisibleCells impostato su true
            ExportTableOptions exportOptions = new ExportTableOptions
            {
                PlotVisibleCells = true,
                PlotVisibleColumns = true,
                PlotVisibleRows = true
            };

            // Esporta solo le celle visibili
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 3, exportOptions);

            // Visualizza i dati esportati (dovrebbero essere esportate solo le celle visibili)
            Console.WriteLine("Exported Data:");
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Vedi anche

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


