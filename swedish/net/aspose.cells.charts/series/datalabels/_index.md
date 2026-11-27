---
title: "Series.DataLabels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series-egenskap. Representerar DataLabels-objektet för den angivna ASeries"
type: docs
url: /sv/net/aspose.cells.charts/series/datalabels/
---
## Series.DataLabels property

Representerar DataLabels-objektet för den angivna ASeries.

```csharp
public DataLabels DataLabels { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyDataLabelsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet och lägg till exempeldata
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Products");
            dataSheet.Cells["B1"].PutValue("Users");
            dataSheet.Cells["A2"].PutValue("Aspose.Cells");
            dataSheet.Cells["B2"].PutValue(10000);
            dataSheet.Cells["A3"].PutValue("Aspose.Slides");
            dataSheet.Cells["B3"].PutValue(8000);
            dataSheet.Cells["A4"].PutValue("Aspose.Words");
            dataSheet.Cells["B4"].PutValue(12000);

            // Lägg till ett diagramblad och skapa ett pajdiagram
            Worksheet chartSheet = workbook.Worksheets[workbook.Worksheets.Add(SheetType.Chart)];
            Chart chart = chartSheet.Charts[chartSheet.Charts.Add(ChartType.Pie, 7, 0, 20, 6)];

            // Lägg till seriedata och konfigurera datamärkningar
            Series series = chart.NSeries[chart.NSeries.Add("=Sheet1!$B$2:$B$4", true)];
            series.XValues = "=Sheet1!$A$2:$A$4";
            
            // Konfigurera DataLabels-egenskaper
            series.DataLabels.ShowValue = true;
            series.DataLabels.ShowCategoryName = true;
            series.DataLabels.ShowPercentage = true;
            series.DataLabels.LinkedSource = null; // Explicitly set to null

            // Spara arbetsboken
            workbook.Save("SeriesPropertyDataLabelsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [DataLabels](../../datalabels/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


