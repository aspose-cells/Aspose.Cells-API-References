---
title: "DropBars.Border"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DropBars‑egenskap. Hämtar gräns‑Line"
type: docs
url: /sv/net/aspose.cells.charts/dropbars/border/
---
## DropBars.Border property

Hämtar kant‑[`Line`](../../../aspose.cells.drawing/line/).

```csharp
public Line Border { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DropBarsPropertyBorderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Lägg till ett linjediagram
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till dataserier i diagrammet
            chart.NSeries.Add("A1:B3", true);

            // Aktivera upp/ner-staplar
            chart.NSeries[0].HasUpDownBars = true;

            try
            {
                // Åtkomst till DropBars-objekten
                DropBars upBars = chart.NSeries[0].UpBars;
                DropBars downBars = chart.NSeries[0].DownBars;

                // Visa aktuella kantegenskaper (skrivskyddad åtkomst)
                Console.WriteLine("Up Bars Border Color: " + upBars.Border.Color);
                Console.WriteLine("Up Bars Border Style: " + upBars.Border.Style);
                Console.WriteLine("Up Bars Border Weight: " + upBars.Border.WeightPt);
                Console.WriteLine("Up Bars Border Visibility: " + upBars.Border.IsVisible);

                Console.WriteLine("\nDown Bars Border Color: " + downBars.Border.Color);
                Console.WriteLine("Down Bars Border Style: " + downBars.Border.Style);
                Console.WriteLine("Down Bars Border Weight: " + downBars.Border.WeightPt);
                Console.WriteLine("Down Bars Border Visibility: " + downBars.Border.IsVisible);

                // Ändra kantegenskaper (eftersom Line inte är skrivskyddad)
                upBars.Border.Color = Color.Blue;
                upBars.Border.Style = LineType.Solid;
                upBars.Border.WeightPt = 2.0;
                upBars.Border.IsVisible = true;

                downBars.Border.Color = Color.Red;
                downBars.Border.Style = LineType.Dash;
                downBars.Border.WeightPt = 1.5;
                downBars.Border.IsVisible = true;

                // Spara arbetsboken
                workbook.Save("DropBarsBorderDemo.xlsx");
                Console.WriteLine("\nBorder properties have been demonstrated and saved to file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [Line](../../../aspose.cells.drawing/line/)
* class [DropBars](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


