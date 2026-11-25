---
title: "DataLabels.IsAutoText"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataLabels. Indica che il testo è generato automaticamente"
type: docs
url: /it/net/aspose.cells.charts/datalabels/isautotext/
---
## DataLabels.IsAutoText property

Indica che il testo è generato automaticamente.

```csharp
public override bool IsAutoText { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyIsAutoTextDemo
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
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Abilita le etichette dei dati
            foreach (Series series in chart.NSeries)
            {
                series.DataLabels.ShowValue = true;
                
                // Dimostrare la proprietà IsAutoText
                foreach (ChartPoint point in series.Points)
                {
                    Console.WriteLine("IsAutoText before setting: " + point.DataLabels.IsAutoText);
                    point.DataLabels.IsAutoText = false;
                    point.DataLabels.Text = "Custom " + point.YValue;
                    Console.WriteLine("IsAutoText after setting: " + point.DataLabels.IsAutoText);
                    Console.WriteLine("DataLabel Text: " + point.DataLabels.Text);
                }
            }
            
            // Salva la cartella di lavoro
            workbook.Save("DataLabelsIsAutoTextDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


