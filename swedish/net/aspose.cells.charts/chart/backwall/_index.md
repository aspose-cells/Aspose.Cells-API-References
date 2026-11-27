---
title: "Chart.BackWall"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart-egenskap. Returnerar ett Walls-objekt som representerar bakväggen i ett 3D-diagram"
type: docs
url: /sv/net/aspose.cells.charts/chart/backwall/
---
## Chart.BackWall property

Returnerar ett [`Walls`](../walls/)‑objekt som representerar bakväggen i ett 3‑D‑diagram.

```csharp
public Walls BackWall { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPropertyBackWallDemo
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
            worksheet.Cells["B2"].PutValue(1200);
            worksheet.Cells["B3"].PutValue(1500);
            worksheet.Cells["B4"].PutValue(1800);

            // Lägg till ett 3D-kolumndiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.SetChartDataRange("A1:B4", true);

            // Se till att det är ett 3D-diagram
            if (chart.Is3D)
            {
                // Hämta BackWall‑objektet
                Walls backWall = chart.BackWall;

                // Visa några egenskaper för BackWall
                Console.WriteLine("BackWall properties:");
                Console.WriteLine("CenterX: " + backWall.CenterX);
                Console.WriteLine("CenterY: " + backWall.CenterY);
                Console.WriteLine("Width: " + backWall.Width);
                Console.WriteLine("Height: " + backWall.Height);

                // Formatera BackWall
                backWall.FillFormat.SetOneColorGradient(
                    System.Drawing.Color.LightBlue, 
                    0.5, // Changed from GradientStyleType to double for degree parameter
                    Aspose.Cells.Drawing.GradientStyleType.Horizontal, 
                    1); // Changed from 0.5 to int for variant parameter

                // Ställ in kantegenskaper
                backWall.Border.Color = System.Drawing.Color.DarkBlue;
                backWall.Border.Weight = Aspose.Cells.Drawing.WeightType.MediumLine;
            }

            // Spara arbetsboken
            workbook.Save("ChartPropertyBackWallDemo.xlsx");
        }
    }
}
```

### Se även

* class [Walls](../../walls/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


