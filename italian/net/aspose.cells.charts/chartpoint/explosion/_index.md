---
title: "ChartPoint.Explosion"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. La distanza di una fetta di torta aperta dal centro del grafico a torta è espressa come percentuale del diametro della torta"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/explosion/
---
## ChartPoint.Explosion property

La distanza di una fetta di torta aperta dal centro del grafico a torta è espressa come percentuale del diametro della torta.

```csharp
public int Explosion { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyExplosionDemo
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

            // Accedi al primo punto del grafico e imposta l'esplosione
            ChartPoint point = chart.NSeries[0].Points[0];
            point.Explosion = 15; // Set explosion distance (15 points)

            // Salva la cartella di lavoro
            workbook.Save("ChartPointExplosionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


