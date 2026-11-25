---
title: "ChartPointCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ChartPointCollection property. Ottiene l'elemento ChartPoint all'indice specificato nella serie"
type: docs
url: /it/net/aspose.cells.charts/chartpointcollection/item/
---
## ChartPointCollection indexer

Ottiene l'elemento [`ChartPoint`](../../chartpoint/) all'indice specificato nella serie.

```csharp
public ChartPoint this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice del punto del grafico nella serie. |

### Valore di ritorno

L'oggetto ChartPoint.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPointCollectionPropertyItemDemo
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

            // Aggiungi un grafico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi a un punto del grafico specifico usando la proprietà Item
            ChartPoint point = chart.NSeries[0].Points[1];
            
            // Modifica il modello di riempimento del punto
            point.Area.FillFormat.Pattern = FillPattern.LightHorizontal;

            // Salva la cartella di lavoro
            workbook.Save("ChartPointCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartPoint](../../chartpoint/)
* class [ChartPointCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


