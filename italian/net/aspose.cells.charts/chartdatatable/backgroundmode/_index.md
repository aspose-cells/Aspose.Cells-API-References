---
title: "ChartDataTable.BackgroundMode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartDataTable. Ottiene e imposta la modalità di visualizzazione dello sfondo"
type: docs
url: /it/net/aspose.cells.charts/chartdatatable/backgroundmode/
---
## ChartDataTable.BackgroundMode property

Ottiene e imposta la modalità di visualizzazione dello sfondo

```csharp
public BackgroundMode BackgroundMode { get; set; }
```

### Esempi

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

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Crea grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configura la tabella dati
            chart.ShowDataTable = true;
            ChartDataTable chartTable = chart.ChartDataTable;
            
            // Dimostra l'uso di BackgroundMode
            chartTable.BackgroundMode = BackgroundMode.Transparent;
            chartTable.Font.Color = Color.Blue;
            chartTable.HasBorderOutline = true;

            workbook.Save("ChartDataTableBackgroundModeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [BackgroundMode](../../backgroundmode/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


