---
title: "Chart.ShowLegend"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart-egenskap. Hämtar eller anger ett värde som indikerar om diagrammets förklaring ska visas. Standard är true"
type: docs
url: /sv/net/aspose.cells.charts/chart/showlegend/
---
## Chart.ShowLegend property

Hämtar eller anger ett värde som indikerar om diagrammets förklaring ska visas. Standard är true.

```csharp
public bool ShowLegend { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyShowLegendDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B1"].PutValue("Quantity");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Visa förklaring som standard (true)
            Console.WriteLine("Legend initially visible: " + chart.ShowLegend);
            
            // Dölj förklaringen
            chart.ShowLegend = false;
            Console.WriteLine("Legend after setting to false: " + chart.ShowLegend);
            
            // Spara arbetsboken
            workbook.Save("ChartLegendExample.xlsx");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


