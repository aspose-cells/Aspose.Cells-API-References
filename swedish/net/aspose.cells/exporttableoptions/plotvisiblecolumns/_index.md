---
title: "ExportTableOptions.PlotVisibleColumns"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExportTableOptions-egenskap. Exporterar endast synliga kolumner"
type: docs
url: /sv/net/aspose.cells/exporttableoptions/plotvisiblecolumns/
---
## ExportTableOptions.PlotVisibleColumns property

Exporterar endast synliga kolumner.

```csharp
public bool PlotVisibleColumns { get; set; }
```

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyPlotVisibleColumnsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata och dölj några kolumner
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["B1"].PutValue("Column2");
            worksheet.Cells["C1"].PutValue("Column3");
            worksheet.Cells["D1"].PutValue("Column4");
            
            for (int i = 2; i <= 5; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue($"Data{i-1}_1");
                worksheet.Cells[$"B{i}"].PutValue($"Data{i-1}_2");
                worksheet.Cells[$"C{i}"].PutValue($"Data{i-1}_3");
                worksheet.Cells[$"D{i}"].PutValue($"Data{i-1}_4");
            }
            
            // Dölj kolumn C
            worksheet.Cells.HideColumn(2);

            // Exportera data med PlotVisibleColumns satt till true
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true;
            options.PlotVisibleColumns = true;

            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 6, 4, options);
            
            // Skriv ut resultaten
            Console.WriteLine("Exported DataTable Columns:");
            foreach (DataColumn column in dataTable.Columns)
            {
                Console.WriteLine(column.ColumnName);
            }
        }
    }
}
```

### Se även

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


