---
title: "ChartFrame.X"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Ottiene o imposta la coordinata x dell'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico"
type: docs
url: /it/net/aspose.cells.charts/chartframe/x/
---
## ChartFrame.X property

Ottiene o imposta la coordinata x dell'angolo in alto a sinistra in unità di 1/4000 dell'area del grafico.

```csharp
[Obsolete("Use ChartFrame.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int X { get; set; }
```

### Osservazioni

Come convertire le unità di 1/4000 in pixel? X in pixel = X * Chart.ChartObject.Width / 4000d;

NOTA: Questo membro è ora obsoleto. Si prega di utilizzare la proprietà ChartFrame.XRatioToChart, invece. X = XRatioToChart * 4000. Questa proprietà sarà rimossa tra 12 mesi a partire da febbraio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyXDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("X Values");
            sheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
            }

            // Aggiungi grafico
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Aggiungi serie e imposta i valori X/Y
            chart.NSeries.Add("Sheet1!B2:B10", true);
            chart.NSeries[0].XValues = "Sheet1!A2:A10";

            // Aggiungi linea di tendenza
            chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "Linear Trend");
            Trendline trendline = chart.NSeries[0].TrendLines[0];
            
            // Configura le etichette dei dati
            trendline.DataLabels.ShowValue = true;
            trendline.DataLabels.Font.Color = Color.Blue;
            
            // Dimostra l'uso della proprietà X
            trendline.DataLabels.X = -500; // Set X position offset
            trendline.DataLabels.Y = 200;  // Set Y position offset

            // Salva la cartella di lavoro
            workbook.Save("ChartFramePropertyXDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


