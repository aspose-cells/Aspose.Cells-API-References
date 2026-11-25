---
title: "Series.SplitValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Restituisce o imposta un valore da utilizzare per determinare quali punti dati sono nella seconda fetta o barra in un grafico a torta di torta o barra di torta"
type: docs
url: /it/net/aspose.cells.charts/series/splitvalue/
---
## Series.SplitValue property

Restituisce o imposta un valore da utilizzare per determinare quali punti dati sono nella seconda torta o barra in un grafico a torta di torta o a barra di torta.

```csharp
public double SplitValue { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySplitValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["A5"].PutValue("Grape");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(10);
            worksheet.Cells["B5"].PutValue(50);

            // Aggiungi un grafico a torta
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Imposta il tipo di divisione e il valore
            chart.NSeries[0].SplitType = ChartSplitType.Custom;
            chart.NSeries[0].SplitValue = 20; // Split points with value <= 20

            // Salva la cartella di lavoro
            workbook.Save("SeriesPropertySplitValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


