---
title: "DataLabels.IsTextWrapped"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataLabels. Ottiene o imposta un valore che indica se il testo è a capo"
type: docs
url: /it/net/aspose.cells.charts/datalabels/istextwrapped/
---
## DataLabels.IsTextWrapped property

Ottiene o imposta un valore che indica se il testo è a capo.

```csharp
public override bool IsTextWrapped { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyIsTextWrappedDemo
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
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(85);
            worksheet.Cells["B4"].PutValue(65);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi alle etichette dei dati
            Aspose.Cells.Charts.DataLabels labels = chart.NSeries[0].DataLabels;
            
            // Mostra etichette dati
            labels.ShowValue = true;
            
            // Dimostra la proprietà IsTextWrapped
            Console.WriteLine("Before setting IsTextWrapped: " + labels.IsTextWrapped);
            labels.IsTextWrapped = true;
            Console.WriteLine("After setting IsTextWrapped: " + labels.IsTextWrapped);

            // Salva la cartella di lavoro
            workbook.Save("DataLabels_IsTextWrapped_Demo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


