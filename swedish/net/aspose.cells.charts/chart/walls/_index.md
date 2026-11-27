---
title: "Chart.Walls"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart-egenskap. Returnerar ett Walls‑objekt som representerar väggarna i ett 3D-diagram"
type: docs
url: /sv/net/aspose.cells.charts/chart/walls/
---
## Chart.Walls property

Returnerar ett `Walls`‑objekt som representerar väggarna i ett 3‑D‑diagram.

```csharp
public Walls Walls { get; }
```

### Anmärkningar

Den här egenskapen gäller inte för 3-D-pie-diagram.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyWallsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(35);

            // Skapa cylindrisk kolumndiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Cylinder, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Konfigurera diagramgrunder
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.IsRectangularCornered = true;
            chart.RotationAngle = 20;

            // Konfigurera väggars egenskaper
            Walls walls = chart.Walls;
            walls.BackgroundColor = Color.LightGray;
            walls.ForegroundColor = Color.Transparent;
            walls.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.Horizontal, 1);

            // Spara resultatet
            workbook.Save("ChartWallsDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


