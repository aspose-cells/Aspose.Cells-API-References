---
title: "DataLabels.SeparatorValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataLabels. Ottiene o imposta il valore separatore usato per le etichette dati su un grafico"
type: docs
url: /it/net/aspose.cells.charts/datalabels/separatorvalue/
---
## DataLabels.SeparatorValue property

Ottiene o imposta il valore del separatore utilizzato per le etichette dati in un grafico.

```csharp
public string SeparatorValue { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertySeparatorValueDemo
    {
        public static void Run()
        {
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

            // Aggiungi grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configura DataLabels
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.ShowCategoryName = true;
            dataLabels.SeparatorValue = " | "; // Demonstrate SeparatorValue property
            dataLabels.Position = LabelPositionType.Center;

            workbook.Save("DataLabelsSeparatorValueDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


