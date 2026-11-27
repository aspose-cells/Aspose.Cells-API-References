---
title: "Chart.GapDepth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart egenskap. Hämtar eller anger avståndet mellan dataserier i ett 3D-diagram som en procentandel av markörbredden. Värdet för denna egenskap måste vara mellan 0 och 500"
type: docs
url: /sv/net/aspose.cells.charts/chart/gapdepth/
---
## Chart.GapDepth property

Hämtar eller anger avståndet mellan dataserierna i ett 3‑D‑diagram, som en procentandel av markörens bredd. Värdet för denna egenskap måste ligga mellan 0 och 500.

```csharp
public int GapDepth { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
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

            // Lägg till ett 3D-kolumndiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ange GapDepth-egenskapen (styr avståndet mellan dataserier i 3D-diagram)
            chart.GapDepth = 150; // Value between 0-500

            // Spara arbetsboken
            workbook.Save("ChartGapDepthDemo.xlsx");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


