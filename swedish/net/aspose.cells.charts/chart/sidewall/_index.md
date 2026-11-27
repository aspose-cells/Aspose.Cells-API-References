---
title: "Chart.SideWall"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart‑egenskap. Returnerar ett Walls‑objekt som representerar sidoväggen på ett 3D‑diagram"
type: docs
url: /sv/net/aspose.cells.charts/chart/sidewall/
---
## Chart.SideWall property

Returnerar ett [`Walls`](../walls/)‑objekt som representerar sidoväggen på ett 3‑D‑diagram.

```csharp
public Walls SideWall { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPropertySideWallDemo
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
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);

            // Lägg till ett 3D-kolumndiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.SetChartDataRange("A1:C4", true);

            // Kom åt SideWall‑egenskapen
            Walls sideWall = chart.SideWall;
            
            // Visa några egenskaper för SideWall
            Console.WriteLine("SideWall properties:");
            Console.WriteLine("Width: " + sideWall.Width);
            Console.WriteLine("Height: " + sideWall.Height);
            Console.WriteLine("Depth: " + sideWall.Depth);

            // Beräkna diagrammet för att uppdatera väggdimensionerna
            chart.Calculate();

            // Visa uppdaterade egenskaper efter beräkning
            Console.WriteLine("\nAfter Calculate():");
            Console.WriteLine("SideWall CenterX: " + sideWall.CenterX);
            Console.WriteLine("SideWall CenterY: " + sideWall.CenterY);
            Console.WriteLine("SideWall WidthPx: " + sideWall.WidthPx);
            Console.WriteLine("SideWall HeightPx: " + sideWall.HeightPx);

            // Spara arbetsboken
            workbook.Save("ChartPropertySideWallDemo.xlsx");
        }
    }
}
```

### Se även

* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


