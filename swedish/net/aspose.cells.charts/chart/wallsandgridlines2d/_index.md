---
title: "Chart.WallsAndGridlines2D"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Diagramegenskap. Sant om rutnätslinjer ritas tvådimensionellt på ett 3D‑diagram"
type: docs
url: /sv/net/aspose.cells.charts/chart/wallsandgridlines2d/
---
## Chart.WallsAndGridlines2D property

Sant om rutnät ritas tvådimensionellt på ett 3‑D‑diagram.

```csharp
public bool WallsAndGridlines2D { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyWallsAndGridlines2DDemo
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
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(15);

            // Lägg till ett stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Demonstrera egenskapen WallsAndGridlines2D
            chart.WallsAndGridlines2D = true; // Show walls and gridlines in 2D
            Console.WriteLine("WallsAndGridlines2D is set to: " + chart.WallsAndGridlines2D);

            // Spara arbetsboken
            workbook.Save("WallsAndGridlines2DDemo.xlsx");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


