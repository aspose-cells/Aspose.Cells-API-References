---
title: "Series.DataLabels"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Rappresenta l'oggetto DataLabels per la ASeries specificata"
type: docs
url: /it/net/aspose.cells.charts/series/datalabels/
---
## Series.DataLabels property

Rappresenta l'oggetto DataLabels per la ASeries specificata.

```csharp
public DataLabels DataLabels { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyDataLabelsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro e aggiungi dati di esempio
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Products");
            dataSheet.Cells["B1"].PutValue("Users");
            dataSheet.Cells["A2"].PutValue("Aspose.Cells");
            dataSheet.Cells["B2"].PutValue(10000);
            dataSheet.Cells["A3"].PutValue("Aspose.Slides");
            dataSheet.Cells["B3"].PutValue(8000);
            dataSheet.Cells["A4"].PutValue("Aspose.Words");
            dataSheet.Cells["B4"].PutValue(12000);

            // Aggiungi un foglio grafico e crea un grafico a torta
            Worksheet chartSheet = workbook.Worksheets[workbook.Worksheets.Add(SheetType.Chart)];
            Chart chart = chartSheet.Charts[chartSheet.Charts.Add(ChartType.Pie, 7, 0, 20, 6)];

            // Aggiungi i dati della serie e configura le etichette dei dati
            Series series = chart.NSeries[chart.NSeries.Add("=Sheet1!$B$2:$B$4", true)];
            series.XValues = "=Sheet1!$A$2:$A$4";
            
            // Configura le proprietà di DataLabels
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShowCategoryName = true;
            series.DataLabels.ShowPercentage = true;
            series.DataLabels.LinkedSource = null; // Explicitly set to null

            // Salva la cartella di lavoro
            workbook.Save("SeriesPropertyDataLabelsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [DataLabels](../../datalabels/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


