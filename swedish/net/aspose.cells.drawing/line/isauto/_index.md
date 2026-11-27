---
title: "Line.IsAuto"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Linjeegenskap. Anger om denna linjestil är automatiskt tilldelad"
type: docs
url: /sv/net/aspose.cells.drawing/line/isauto/
---
## Line.IsAuto property

Indikerar om den här linjestilen är automatiskt tilldelad.

```csharp
public bool IsAuto { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class LinePropertyIsAutoDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            try
            {
                // Lägg till ett linjediagram
                int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
                Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

                // Ange diagrammets dataområde
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";

                // Kom åt linjeegenskaperna för serien
                Aspose.Cells.Charts.Series series = chart.NSeries[0];
                Line line = series.Border;

                // Visa det aktuella IsAuto‑värdet
                Console.WriteLine("Initial IsAuto value: " + line.IsAuto);

                // Ställ in IsAuto till true
                line.IsAuto = true;
                Console.WriteLine("After setting to true, IsAuto value: " + line.IsAuto);

                // Ställ in IsAuto till false
                line.IsAuto = false;
                Console.WriteLine("After setting to false, IsAuto value: " + line.IsAuto);

                // Spara arbetsboken
                workbook.Save("IsAutoDemo.xlsx");
                Console.WriteLine("IsAuto property has been demonstrated successfully.");
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

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


