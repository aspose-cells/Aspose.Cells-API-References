---
title: "Chart.ValueAxis"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Restituisce l'asse Y del grafico"
type: docs
url: /it/net/aspose.cells.charts/chart/valueaxis/
---
## Chart.ValueAxis property

Ottiene l'asse Y del grafico.

```csharp
public Axis ValueAxis { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyValueAxisDemo
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
            worksheet.Cells["B2"].PutValue(100000000);
            worksheet.Cells["B3"].PutValue(200000000);
            worksheet.Cells["B4"].PutValue(300000000);

            // Aggiungi un grafico e imposta il suo intervallo di dati
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Configura le proprietà di ValueAxis
            chart.ValueAxis.DisplayUnit = DisplayUnitType.HundredMillions;
            chart.ValueAxis.Title.Text = "Values (in 100 millions)";
            chart.ValueAxis.MajorUnit = 1;

            // Salva la cartella di lavoro
            workbook.Save("ChartPropertyValueAxisDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


