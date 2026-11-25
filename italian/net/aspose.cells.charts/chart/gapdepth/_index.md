---
title: "Chart.GapDepth"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà del grafico. Ottiene o imposta la distanza tra le serie di dati in un grafico 3D come percentuale della larghezza del marcatore. Il valore di questa proprietà deve essere compreso tra 0 e 500"
type: docs
url: /it/net/aspose.cells.charts/chart/gapdepth/
---
## Chart.GapDepth property

Ottiene o imposta la distanza tra le serie di dati in un grafico 3-D, come percentuale della larghezza del marcatore. Il valore di questa proprietà deve essere compreso tra 0 e 500.

```csharp
public int GapDepth { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyGapDepthDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(180);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(90);
            worksheet.Cells["C3"].PutValue(110);
            worksheet.Cells["C4"].PutValue(130);

            // Aggiungi un grafico a colonne 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Imposta la proprietà GapDepth (controlla la distanza tra le serie di dati nei grafici 3D)
            chart.GapDepth = 150; // Value between 0-500

            // Salva la cartella di lavoro
            workbook.Save("ChartGapDepthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


