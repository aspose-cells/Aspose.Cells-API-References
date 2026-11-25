---
title: "Chart.SeriesAxis"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà del grafico. Ottiene l'asse delle serie del grafico"
type: docs
url: /it/net/aspose.cells.charts/chart/seriesaxis/
---
## Chart.SeriesAxis property

Ottiene l'asse delle serie del grafico.

```csharp
public Axis SeriesAxis { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySeriesAxisDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Series");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C1"].PutValue("Product B");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);

            // Aggiungi un grafico a colonne raggruppate 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B1:C4", true);

            // Accedi e configura l'asse delle serie
            Axis seriesAxis = chart.SeriesAxis;
            seriesAxis.Title.Text = "Product Series";
            seriesAxis.Title.Font.Size = 12;
            seriesAxis.Title.Font.IsBold = true;
            seriesAxis.MajorTickMark = TickMarkType.Cross;
            seriesAxis.MinorTickMark = TickMarkType.Outside;

            // Salva la cartella di lavoro
            workbook.Save("ChartPropertySeriesAxisDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


