---
title: "Chart.AutoScaling"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Vero se Microsoft Excel scala un grafico 3D in modo che sia più vicino in dimensione al grafico 2D equivalente. La proprietà RightAngleAxes deve essere True"
type: docs
url: /it/net/aspose.cells.charts/chart/autoscaling/
---
## Chart.AutoScaling property

Vero se Microsoft Excel scala un grafico 3-D in modo che sia più vicino in dimensione al grafico 2-D equivalente. La proprietà RightAngleAxes deve essere True.

```csharp
public bool AutoScaling { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyAutoScalingDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Dimostra la proprietà AutoScaling
            chart.AutoScaling = false;
            Console.WriteLine("Chart AutoScaling is set to: " + chart.AutoScaling);

            // Salva la cartella di lavoro
            workbook.Save("ChartAutoScalingDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


