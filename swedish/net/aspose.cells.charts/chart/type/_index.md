---
title: "Chart.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Diagramegenskap. Hämtar eller anger en diagramtyp"
type: docs
url: /sv/net/aspose.cells.charts/chart/type/
---
## Chart.Type property

Hämtar eller anger diagrammets typ.

```csharp
public ChartType Type { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Lägg till ett radardiagram
            int chartIndex = sheet.Charts.Add(ChartType.Radar, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Demonstrera användning av Type-egenskapen
            Console.WriteLine("Chart type is: " + chart.Type);
            
            // Ändra diagramtyp till Kolumn
            chart.Type = ChartType.Column;
            Console.WriteLine("Chart type changed to: " + chart.Type);
        }
    }
}
```

### Se även

* enum [ChartType](../../charttype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


