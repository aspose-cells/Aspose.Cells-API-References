---
title: "ExportTableOptions.PlotVisibleColumns"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExportTableOptions-Eigenschaft. Exportiert nur sichtbare Spalten"
type: docs
url: /de/net/aspose.cells/exporttableoptions/plotvisiblecolumns/
---
## ExportTableOptions.PlotVisibleColumns property

Exportiert nur sichtbare Spalten.

```csharp
public bool PlotVisibleColumns { get; set; }
```

### Beispiele

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
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten hinzufügen und einige Spalten ausblenden
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
            
            // Spalte C ausblenden
            worksheet.Cells.HideColumn(2);

            // Daten exportieren mit PlotVisibleColumns auf true gesetzt
            ExportTableOptions options = new ExportTableOptions();
            options.ExportColumnName = true;
            options.PlotVisibleColumns = true;

            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 6, 4, options);
            
            // Ergebnisse ausgeben
            Console.WriteLine("Exported DataTable Columns:");
            foreach (DataColumn column in dataTable.Columns)
            {
                Console.WriteLine(column.ColumnName);
            }
        }
    }
}
```

### Siehe auch

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


