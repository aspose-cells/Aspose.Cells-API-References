---
title: "Chart.Perspective"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Diagramegenskap. Returnerar eller anger perspektivet för den tredimensionella diagramvyn. Måste vara mellan 0 och 100. Denna egenskap ignoreras om RightAngleAxes‑egenskapen är True"
type: docs
url: /sv/net/aspose.cells.charts/chart/perspective/
---
## Chart.Perspective property

Returnerar eller anger perspektivet för den tredimensionella diagramvyn. Måste vara mellan 0 och 100. Denna egenskap ignoreras om egenskapen RightAngleAxes är True.

```csharp
public short Perspective { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPerspectiveDemo
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
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Lägg till ett 3D-kolumndiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ange perspektivegenskaper för 3D‑diagrammet
            chart.Perspective = 30; // Perspective angle (0-100)
            chart.RotationAngle = 15; // Rotation angle
            chart.Elevation = 20; // Elevation angle
            chart.RightAngleAxes = false; // Enable perspective projection
            chart.AutoScaling = true; // Auto scale the chart

            // Spara arbetsboken
            workbook.Save("ChartPerspectiveDemo.xlsx");

            Console.WriteLine("Chart with perspective settings created successfully.");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


