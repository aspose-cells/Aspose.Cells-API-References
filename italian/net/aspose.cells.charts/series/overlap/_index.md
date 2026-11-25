---
title: "Series.Overlap"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Specifica come sono posizionate le barre e le colonne. Può essere un valore compreso tra 100 e 100. Si applica solo ai grafici a barre 2D e a colonne 2D"
type: docs
url: /it/net/aspose.cells.charts/series/overlap/
---
## Series.Overlap property

Specifica come sono posizionate le barre e le colonne. Può essere un valore compreso tra -100 e 100. Si applica solo ai grafici a barre 2-D e a colonne 2-D.

```csharp
public short Overlap { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyOverlapDemo
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
            sheet.Cells["B1"].PutValue("Series1");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            sheet.Cells["C1"].PutValue("Series2");
            sheet.Cells["C2"].PutValue(15);
            sheet.Cells["C3"].PutValue(25);
            sheet.Cells["C4"].PutValue(35);

            // Aggiungi un grafico a colonne raggruppate
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Imposta la proprietà overlap per la prima serie
            chart.NSeries[0].Overlap = -40;

            // Salva la cartella di lavoro
            workbook.Save("SeriesOverlapDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


