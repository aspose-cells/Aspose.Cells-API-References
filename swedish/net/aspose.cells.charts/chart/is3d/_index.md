---
title: "Chart.Is3D"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart-egenskap. Anger om diagrammet är ett 3D-diagram"
type: docs
url: /sv/net/aspose.cells.charts/chart/is3d/
---
## Chart.Is3D property

Anger om diagrammet är ett 3d-diagram.

```csharp
public bool Is3D { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPropertyIs3DDemo
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
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);
            worksheet.Cells["B5"].PutValue(2100);

            // Lägg till ett stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 6, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange dataområde för diagrammet
            chart.SetChartDataRange("A1:B5", true);

            // Visa det aktuella Is3D-värdet
            Console.WriteLine("Current Is3D value: " + chart.Is3D);

            // Skapa en 3D-version av diagrammet
            int chart3DIndex = worksheet.Charts.Add(ChartType.Column3D, 6, 12, 20, 22);
            Chart chart3D = worksheet.Charts[chart3DIndex];
            chart3D.SetChartDataRange("A1:B5", true);

            // Visa 3D-diagrammets Is3D-värde
            Console.WriteLine("3D Chart Is3D value: " + chart3D.Is3D);

            // Spara arbetsboken
            workbook.Save("ChartPropertyIs3DDemo.xlsx");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


