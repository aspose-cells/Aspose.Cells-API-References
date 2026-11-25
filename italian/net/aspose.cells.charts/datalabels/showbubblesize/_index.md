---
title: "DataLabels.ShowBubbleSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataLabels. Rappresenta il comportamento di visualizzazione del valore percentuale dell'etichetta dati di un grafico specificato. True visualizza il valore percentuale. False nasconde il valore percentuale"
type: docs
url: /it/net/aspose.cells.charts/datalabels/showbubblesize/
---
## DataLabels.ShowBubbleSize property

Rappresenta il comportamento di visualizzazione del valore percentuale dell'etichetta dati di un grafico specificato. True visualizza il valore percentuale. False lo nasconde.

```csharp
public bool ShowBubbleSize { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowBubbleSizeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico a bolle
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C1"].PutValue("Size");
            worksheet.Cells["C2"].PutValue(5);
            worksheet.Cells["C3"].PutValue(10);
            worksheet.Cells["C4"].PutValue(15);

            // Aggiungi un grafico a bolle
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Aggiungi serie al grafico
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Imposta le dimensioni delle bolle per la serie
            Series series = chart.NSeries[seriesIndex];
            series.BubbleSizes = "C2:C4";

            // Accedi alle DataLabels della serie
            DataLabels dataLabels = series.DataLabels;

            // Dimostrare la proprietà ShowBubbleSize
            dataLabels.ShowBubbleSize = true; // Show bubble size in data labels
            dataLabels.ShowValue = true;      // Also show values for clarity

            // Salva la cartella di lavoro
            workbook.Save("DataLabelsShowBubbleSizeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


