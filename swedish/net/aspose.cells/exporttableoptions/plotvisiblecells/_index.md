---
title: "ExportTableOptions.PlotVisibleCells"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExportTableOptions egenskap. Exporterar endast synliga celler"
type: docs
url: /sv/net/aspose.cells/exporttableoptions/plotvisiblecells/
---
## ExportTableOptions.PlotVisibleCells property

Exporterar endast synliga celler.

```csharp
public bool PlotVisibleCells { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata med några dolda rader/kolumner
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["C1"].PutValue("Header3");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue("Data3");
            
            // Dölj rad 2 och kolumn B (index 1)
            worksheet.Cells.HideRow(1);
            worksheet.Cells.HideColumn(1);

            // Skapa exportalternativ med PlotVisibleCells satt till true
            ExportTableOptions exportOptions = new ExportTableOptions
            {
                PlotVisibleCells = true,
                PlotVisibleColumns = true,
                PlotVisibleRows = true
            };

            // Exportera endast synliga celler
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 3, exportOptions);

            // Visa de exporterade data (endast synliga celler bör exporteras)
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

### Se även

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


