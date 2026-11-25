---
title: "Chart.Legend"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Ottiene la legenda del grafico"
type: docs
url: /it/net/aspose.cells.charts/chart/legend/
---
## Chart.Legend property

Ottiene la legenda del grafico.

```csharp
public Legend Legend { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyLegendDemo
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

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Personalizza la legenda
            chart.Legend.IsAutomaticSize = false;
            chart.Legend.Position = LegendPositionType.Bottom;
            chart.Legend.Width = 400;
            chart.Legend.Height = 50;
            chart.Legend.Font.Size = 12;
            chart.Legend.Font.IsBold = true;

            // Salva la cartella di lavoro
            workbook.Save("ChartLegendDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Legend](../../legend/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


