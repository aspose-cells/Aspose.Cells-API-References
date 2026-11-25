---
title: "DataLabels.ShowCellRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà DataLabels. Indica se mostrare l'intervallo di celle come etichette dati"
type: docs
url: /it/net/aspose.cells.charts/datalabels/showcellrange/
---
## DataLabels.ShowCellRange property

Indica se mostrare l'intervallo di celle come etichette dati.

```csharp
public bool ShowCellRange { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowCellRangeDemo
    {
        public static void Run()
        {
            // Crea cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["C2"].PutValue("100 units");
            worksheet.Cells["C3"].PutValue("200 units");

            // Crea grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Configura le etichette dati con ShowCellRange
            var series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShowCellRange = true;
            series.DataLabels.LinkedSource = "C2:C3";
            series.DataLabels.Font.Color = Color.Blue;

            // Salva la cartella di lavoro
            workbook.Save("DataLabelsShowCellRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


