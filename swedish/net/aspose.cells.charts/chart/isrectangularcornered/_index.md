---
title: "Chart.IsRectangularCornered"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Diagramegenskap. Hämtar eller anger ett värde som indikerar om diagramområdet har rektangulära hörn. Standard är true"
type: docs
url: /sv/net/aspose.cells.charts/chart/isrectangularcornered/
---
## Chart.IsRectangularCornered property

Hämtar eller anger ett värde som indikerar om diagramområdet har rektangulära hörn. Standard är true.

```csharp
public bool IsRectangularCornered { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyIsRectangularCorneredDemo
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

            // Lägg till ett stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Demonstrera egenskapen IsRectangularCornered
            Console.WriteLine("Default IsRectangularCornered: " + chart.IsRectangularCornered);
            
            // Ställ in på true för att göra diagramhörnen rektangulära
            chart.IsRectangularCornered = true;
            Console.WriteLine("After setting IsRectangularCornered to true: " + chart.IsRectangularCornered);

            // Spara arbetsboken
            workbook.Save("ChartPropertyIsRectangularCorneredDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


