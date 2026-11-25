---
title: "DataLabels.ShowLegendKey"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataLabels. Rappresenta il comportamento di visualizzazione della chiave della legenda dell'etichetta dati di un grafico specificato. True se la chiave della legenda dell'etichetta dati è visibile"
type: docs
url: /it/net/aspose.cells.charts/datalabels/showlegendkey/
---
## DataLabels.ShowLegendKey property

Rappresenta il comportamento di visualizzazione della chiave legenda dell'etichetta dati di un grafico specificato. True se la chiave legenda dell'etichetta dati è visibile.

```csharp
public bool ShowLegendKey { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowLegendKeyDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni le etichette dati
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            
            // Imposta ShowLegendKey su true
            dataLabels.ShowLegendKey = true;
            Console.WriteLine("ShowLegendKey set to: " + dataLabels.ShowLegendKey);

            // Salva la cartella di lavoro
            workbook.Save("DataLabelsShowLegendKeyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


