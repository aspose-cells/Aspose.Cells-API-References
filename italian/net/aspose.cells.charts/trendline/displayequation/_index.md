---
title: "Trendline.DisplayEquation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Trendline. Indica se l'equazione della trendline è visualizzata sul grafico nella stessa etichetta dati del valore R quadrato. Impostare questa proprietà su True attiva automaticamente le etichette dati"
type: docs
url: /it/net/aspose.cells.charts/trendline/displayequation/
---
## Trendline.DisplayEquation property

Indica se l'equazione della linea di tendenza è visualizzata sul grafico (nella stessa etichetta dati del valore R-quadrato). Impostare questa proprietà su True attiva automaticamente le etichette dati.

```csharp
public bool DisplayEquation { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyDisplayEquationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            // Crea grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie e trendline
            chart.NSeries.Add("A1:B4", true);
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Configura le proprietà della trendline
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = false;
            trendline.Color = Color.Blue;

            workbook.Save("TrendlineDisplayEquationDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


