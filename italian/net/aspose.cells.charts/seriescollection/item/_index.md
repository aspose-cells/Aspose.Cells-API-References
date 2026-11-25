---
title: "SeriesCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SeriesCollection. Ottiene l'elemento Series all'indice specificato"
type: docs
url: /it/net/aspose.cells.charts/seriescollection/item/
---
## SeriesCollection indexer

Ottiene l'elemento [`Series`](../../series/) all'indice specificato.

```csharp
public Series this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice a base zero dell'elemento. |

### Valore di ritorno

L'elemento all'indice specificato.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            sheet.Cells["A1"].PutValue("Series");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["B1"].PutValue("Values");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi alla prima serie e al suo primo punto usando la proprietà Item
            Series series = chart.NSeries[0];
            ChartPoint point = series.Points[0];

            // Personalizza l'aspetto del punto
            point.Area.FillFormat.SetTwoColorGradient(System.Drawing.Color.Blue, System.Drawing.Color.White, GradientStyleType.Vertical, 2);
            point.Area.FillFormat.FillType = FillType.Solid;

            // Salva la cartella di lavoro
            workbook.Save("SeriesCollectionPropertyItemDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [Series](../../series/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


