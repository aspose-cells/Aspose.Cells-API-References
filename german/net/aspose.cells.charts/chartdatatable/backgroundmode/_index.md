---
title: "ChartDataTable.BackgroundMode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ChartDataTable-Eigenschaft. Ruft den Anzeigemodus des Hintergrunds ab und legt ihn fest"
type: docs
url: /de/net/aspose.cells.charts/chartdatatable/backgroundmode/
---
## ChartDataTable.BackgroundMode property

Liest und setzt den Anzeigemodus des Hintergrunds

```csharp
public BackgroundMode BackgroundMode { get; set; }
```

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyBackgroundModeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Diagramm erstellen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Datentabelle konfigurieren
            chart.ShowDataTable = true;
            ChartDataTable chartTable = chart.ChartDataTable;
            
            // Demonstrieren Sie die Verwendung von BackgroundMode
            chartTable.BackgroundMode = BackgroundMode.Transparent;
            chartTable.Font.Color = Color.Blue;
            chartTable.HasBorderOutline = true;

            workbook.Save("ChartDataTableBackgroundModeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [BackgroundMode](../../backgroundmode/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


