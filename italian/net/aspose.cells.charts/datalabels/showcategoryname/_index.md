---
title: "DataLabels.ShowCategoryName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataLabels. Rappresenta il comportamento di visualizzazione del nome della categoria dell'etichetta dati di un grafico specificato. True per visualizzare il nome della categoria per le etichette dati su un grafico. False per nascondere"
type: docs
url: /it/net/aspose.cells.charts/datalabels/showcategoryname/
---
## DataLabels.ShowCategoryName property

Rappresenta il comportamento di visualizzazione del nome della categoria dell'etichetta dati di un grafico specificato. True per visualizzare il nome della categoria per le etichette dati in un grafico. False per nasconderlo.

```csharp
public bool ShowCategoryName { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowCategoryNameDemo
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

            // Abilita le etichette dati e imposta le proprietà
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.ShowCategoryName = true;
            dataLabels.SeparatorType = DataLabelsSeparatorType.Semicolon;

            // Salva la cartella di lavoro
            workbook.Save("DataLabelsShowCategoryNameDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


