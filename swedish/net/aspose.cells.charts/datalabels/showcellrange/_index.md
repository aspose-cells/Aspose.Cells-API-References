---
title: "DataLabels.ShowCellRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DataLabels-egenskap. Anger om cellintervall ska visas som dataetiketter"
type: docs
url: /sv/net/aspose.cells.charts/datalabels/showcellrange/
---
## DataLabels.ShowCellRange property

Indikerar om cellområdet ska visas som datamärken.

```csharp
public bool ShowCellRange { get; set; }
```

### Exempel

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
            // Skapa arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ange exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["C2"].PutValue("100 units");
            worksheet.Cells["C3"].PutValue("200 units");

            // Skapa diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Konfigurera dataetiketter med ShowCellRange
            var series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShowCellRange = true;
            series.DataLabels.LinkedSource = "C2:C3";
            series.DataLabels.Font.Color = Color.Blue;

            // Spara arbetsboken
            workbook.Save("DataLabelsShowCellRangeDemo.xlsx");
        }
    }
}
```

### Se även

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


