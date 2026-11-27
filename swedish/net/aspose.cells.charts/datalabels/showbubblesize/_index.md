---
title: "DataLabels.ShowBubbleSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataLabels-egenskap. Representerar ett specificerat diagramdataetikett-procentvärdes visningsbeteende. Sant visar procentvärdet. Falskt döljer procentvärdet"
type: docs
url: /sv/net/aspose.cells.charts/datalabels/showbubblesize/
---
## DataLabels.ShowBubbleSize property

Representerar ett specificerat diagrammets visningsbeteende för datamärkets procentvärde. Sant visar procentvärdet. Falskt döljer procentvärdet.

```csharp
public bool ShowBubbleSize { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowBubbleSizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för bubbeldiagram
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C1"].PutValue("Size");
            worksheet.Cells["C2"].PutValue(5);
            worksheet.Cells["C3"].PutValue(10);
            worksheet.Cells["C4"].PutValue(15);

            // Lägg till ett bubbeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till serier i diagrammet
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Ange bubblestorlekar för serien
            Series series = chart.NSeries[seriesIndex];
            series.BubbleSizes = "C2:C4";

            // Kom åt DataLabels för serien
            DataLabels dataLabels = series.DataLabels;

            // Demonstrera egenskapen ShowBubbleSize
            dataLabels.ShowBubbleSize = true; // Show bubble size in data labels
            dataLabels.ShowValue = true;      // Also show values for clarity

            // Spara arbetsboken
            workbook.Save("DataLabelsShowBubbleSizeDemo.xlsx");
        }
    }
}
```

### Se även

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


