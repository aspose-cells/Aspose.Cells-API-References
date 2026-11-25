---
title: "DataLabels.ShowPercentage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataLabels. Rappresenta il comportamento di visualizzazione del valore percentuale dell'etichetta dati di un grafico specificato. True visualizza il valore percentuale. False per nascondere"
type: docs
url: /it/net/aspose.cells.charts/datalabels/showpercentage/
---
## DataLabels.ShowPercentage property

Rappresenta il comportamento di visualizzazione del valore percentuale dell'etichetta dati di un grafico specificato. True visualizza il valore percentuale. False lo nasconde.

```csharp
public bool ShowPercentage { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowPercentageDemo
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

            // Aggiungi un grafico a torta
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Abilita le etichette dati e mostra la percentuale
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowPercentage = true;
            dataLabels.ShowValue = false;

            // Salva la cartella di lavoro
            workbook.Save("DataLabelsShowPercentageDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


