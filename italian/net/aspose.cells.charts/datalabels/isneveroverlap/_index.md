---
title: "DataLabels.IsNeverOverlap"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataLabels. Indica se Datalabels non si sovrappongono mai durante la conversione di un Pie Chart in immagine. Nota questa proprietà è significativa solo quando un Pie Chart è convertito in immagine"
type: docs
url: /it/net/aspose.cells.charts/datalabels/isneveroverlap/
---
## DataLabels.IsNeverOverlap property

Indica se le etichette dati non si sovrappongono mai durante la creazione di un'immagine di grafico a torta. Nota: questa proprietà è significativa solo quando si crea un'immagine di grafico a torta.

```csharp
public bool IsNeverOverlap { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyIsNeverOverlapDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico a colonne
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Abilita le etichette dei dati
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;

            // Ottieni le etichette dati e imposta la proprietà IsNeverOverlap
            DataLabels dataLabels = series.DataLabels;
            Console.WriteLine("Default IsNeverOverlap value: " + dataLabels.IsNeverOverlap);
            
            // Imposta IsNeverOverlap su true
            dataLabels.IsNeverOverlap = true;
            Console.WriteLine("After setting IsNeverOverlap: " + dataLabels.IsNeverOverlap);

            // Salva la cartella di lavoro
            workbook.Save("DataLabelsIsNeverOverlapDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


