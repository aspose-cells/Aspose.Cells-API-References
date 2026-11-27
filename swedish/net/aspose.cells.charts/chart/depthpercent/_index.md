---
title: "Chart.DepthPercent"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart‑egenskap. Representerar djupet på ett 3D‑diagram som en procentandel av diagrammets bredd mellan 20 och 2000 procent"
type: docs
url: /sv/net/aspose.cells.charts/chart/depthpercent/
---
## Chart.DepthPercent property

Representerar djupet på ett 3‑D‑diagram som en procentandel av diagrammets bredd (mellan 20 och 2000 procent).

```csharp
public int DepthPercent { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
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

            // Lägg till ett 3D-kolumndiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ställ in DepthPercent‑egenskapen (styr djupet på ett 3D‑diagram som en procentandel av diagrammets bredd)
            chart.DepthPercent = 150; // 150% depth

            // Spara arbetsboken
            workbook.Save("ChartDepthPercentDemo.xlsx");

            Console.WriteLine("Chart with DepthPercent 150% created successfully.");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


