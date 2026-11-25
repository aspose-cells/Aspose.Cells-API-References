---
title: "Chart.DepthPercent"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Rappresenta la profondità di un grafico 3D come percentuale della larghezza del grafico tra il 20% e il 2000%"
type: docs
url: /it/net/aspose.cells.charts/chart/depthpercent/
---
## Chart.DepthPercent property

Rappresenta la profondità di un grafico 3-D come percentuale della larghezza del grafico (tra il 20 e il 2000 percento).

```csharp
public int DepthPercent { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyDepthPercentDemo
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
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);

            // Aggiungi un grafico a colonne 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Imposta la proprietà DepthPercent (controlla la profondità del grafico 3D come percentuale della larghezza del grafico)
            chart.DepthPercent = 150; // 150% depth

            // Salva la cartella di lavoro
            workbook.Save("ChartDepthPercentDemo.xlsx");

            Console.WriteLine("Chart with DepthPercent 150% created successfully.");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


