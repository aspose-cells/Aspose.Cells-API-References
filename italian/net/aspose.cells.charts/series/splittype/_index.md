---
title: "Series.SplitType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Restituisce o imposta un valore che determina quali punti dati sono nella seconda torta o barra in un grafico torta di torta o barra di torta."
type: docs
url: /it/net/aspose.cells.charts/series/splittype/
---
## Series.SplitType property

Restituisce o imposta un valore che determina quali punti dati sono nella seconda torta o barra in un grafico a torta di torta o a barra di torta.

```csharp
public ChartSplitType SplitType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySplitTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico a torta
            int chartIndex = sheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Imposta il tipo di divisione per la prima serie
            chart.NSeries[0].SplitType = ChartSplitType.Position;

            // Salva la cartella di lavoro
            workbook.Save("SeriesPropertySplitTypeDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* enum [ChartSplitType](../../chartsplittype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


