---
title: "DataLabels.BackgroundMode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataLabels. Ottiene e imposta la modalità di visualizzazione dello sfondo"
type: docs
url: /it/net/aspose.cells.charts/datalabels/backgroundmode/
---
## DataLabels.BackgroundMode property

Ottiene e imposta la modalità di visualizzazione dello sfondo

```csharp
public BackgroundMode BackgroundMode { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyBackgroundModeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(5);

            // Crea un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // Ottieni le etichette dati
            Aspose.Cells.Charts.DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;

            // Dimostra la proprietà BackgroundMode
            dataLabels.BackgroundMode = BackgroundMode.Automatic; // Automatic background
            Console.WriteLine("BackgroundMode set to Automatic");

            // Salva la cartella di lavoro
            workbook.Save("DataLabelsBackgroundModeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [BackgroundMode](../../backgroundmode/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


