---
title: "ErrorBar.ShowMarkerTTop"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ErrorBar. Indica se formattare le barre di errore con un Ttop"
type: docs
url: /it/net/aspose.cells.charts/errorbar/showmarkerttop/
---
## ErrorBar.ShowMarkerTTop property

Indica se formattare le barre di errore con una T superiore.

```csharp
public bool ShowMarkerTTop { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyShowMarkerTTopDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi dati di esempio
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            cells["B1"].PutValue(2);
            cells["B2"].PutValue(3);
            cells["B3"].PutValue(1);

            // Crea un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta i dati del grafico
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries.CategoryData = "B1:B3";

            // Configura le barre di errore per la prima serie
            Series series = chart.NSeries[0];
            series.YErrorBar.DisplayType = ErrorBarDisplayType.Both;
            series.YErrorBar.Type = ErrorBarType.Percent;
            series.YErrorBar.Amount = 10;
            
            // Dimostra la proprietà ShowMarkerTTop
            series.YErrorBar.ShowMarkerTTop = true;
            series.YErrorBar.Color = System.Drawing.Color.Red;
            series.YErrorBar.Style = LineType.DashDot;

            // Salva la cartella di lavoro
            workbook.Save("ErrorBarShowMarkerTTopDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


