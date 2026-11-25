---
title: "LegendEntry.BackgroundMode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LegendEntry. Ottiene e imposta la modalità di visualizzazione dello sfondo"
type: docs
url: /it/net/aspose.cells.charts/legendentry/backgroundmode/
---
## LegendEntry.BackgroundMode property

Ottiene e imposta la modalità di visualizzazione dello sfondo

```csharp
public BackgroundMode BackgroundMode { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyBackgroundModeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");

            // Crea grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B2", true);
            chart.NSeries.CategoryData = "C1:C2";

            // Configura voce della legenda
            LegendEntry legendEntry = chart.NSeries[0].LegendEntry;
            legendEntry.BackgroundMode = BackgroundMode.Opaque;
            legendEntry.Font.Color = System.Drawing.Color.Blue;

            workbook.Save("LegendEntryBackgroundModeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [BackgroundMode](../../backgroundmode/)
* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


