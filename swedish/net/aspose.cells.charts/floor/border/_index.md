---
title: "Floor.Border"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Floor-egenskap. Hämtar eller anger gränslinjen Line"
type: docs
url: /sv/net/aspose.cells.charts/floor/border/
---
## Floor.Border property

Hämtar eller anger gränsen [`Line`](../../../aspose.cells.drawing/line/).

```csharp
public Line Border { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FloorPropertyBorderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett 3D-kolumndiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Hämta golvet för diagrammet
            Floor floor = chart.Floor;

            // Ställ in kantens egenskaper genom att ändra befintlig kant istället för att skapa en ny
            floor.Border.Color = Color.Red;
            floor.Border.Weight = WeightType.MediumLine;
            floor.Border.DashType = MsoLineDashStyle.DashDot;
            floor.Border.IsVisible = true;
            floor.Border.Transparency = 0.5;

            // Spara arbetsboken
            workbook.Save("FloorBorderDemo.xlsx");
        }
    }
}
```

### Se även

* class [Line](../../../aspose.cells.drawing/line/)
* class [Floor](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


