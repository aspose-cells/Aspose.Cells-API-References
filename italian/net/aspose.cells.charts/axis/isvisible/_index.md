---
title: "Axis.IsVisible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Indica se l'asse è visibile"
type: docs
url: /it/net/aspose.cells.charts/axis/isvisible/
---
## Axis.IsVisible property

Rappresenta se l'asse è visibile.

```csharp
public bool IsVisible { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Aggiungi una serie di asse secondario
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries[1].PlotOnSecondAxis = true;

            // Dimostra la proprietà IsVisible
            Console.WriteLine("Secondary Value Axis Visible: " + chart.SecondValueAxis.IsVisible);
            
            // Nascondi l'asse secondario
            chart.SecondValueAxis.IsVisible = false;
            Console.WriteLine("After setting to false - Secondary Value Axis Visible: " + chart.SecondValueAxis.IsVisible);

            // Salva la cartella di lavoro
            workbook.Save("AxisIsVisibleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


