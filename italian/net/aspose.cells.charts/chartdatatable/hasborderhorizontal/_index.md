---
title: "ChartDataTable.HasBorderHorizontal"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartDataTable. True se la tabella dati del grafico ha bordi orizzontali delle celle"
type: docs
url: /it/net/aspose.cells.charts/chartdatatable/hasborderhorizontal/
---
## ChartDataTable.HasBorderHorizontal property

Vero se la tabella dati del grafico ha bordi orizzontali delle celle

```csharp
[Obsolete("Use ChartDataTable.HasHorizontalBorder property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasBorderHorizontal { get; set; }
```

### Osservazioni

NOTE: Questa proprietà è ora obsoleta. Invece, si prega di utilizzare la proprietà ChartDataTable.HasHorizontalBorder. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasBorderHorizontalDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            chart.ShowDataTable = true;

            ChartDataTable chartTable = chart.ChartDataTable;
            chartTable.HasBorderHorizontal = true;
            chartTable.HasBorderVertical = false;
            chartTable.HasBorderOutline = false;

            workbook.Save("ChartDataTable_HasBorderHorizontal.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


