---
title: "Chart.FirstSliceAngle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Diagramegenskap. Hämtar eller anger vinkeln för den första paj- eller donutdiagrammets segment i grader medurs från vertikalen. Gäller endast för paj-, 3D-paj- och donutdiagram 0 till 360"
type: docs
url: /sv/net/aspose.cells.charts/chart/firstsliceangle/
---
## Chart.FirstSliceAngle property

Hämtar eller anger vinkeln på den första sektorn i ett cirkeldiagram eller donutdiagram, i grader (medurs från vertikal). Gäller endast cirkel-, 3‑D‑cirkeldiagram och donutdiagram, 0 till 360.

```csharp
public int FirstSliceAngle { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyFirstSliceAngleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Lägg till pajdiagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Pie, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Ange första segmentvinkeln till 45 grader
            chart.FirstSliceAngle = 45;
            
            // Spara arbetsboken
            workbook.Save("PieChartWithFirstSliceAngle.xlsx");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


