---
title: "Chart.GapWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart egenskap. Returnerar eller anger avståndet mellan stapel- eller kolumnkluster som en procentandel av stapel- eller kolumnbredden. Värdet för denna egenskap måste vara mellan 0 och 500"
type: docs
url: /sv/net/aspose.cells.charts/chart/gapwidth/
---
## Chart.GapWidth property

Returnerar eller anger avståndet mellan stapel‑ eller kolumnkluster, som en procentandel av stapelns eller kolumnens bredd. Värdet för denna egenskap måste ligga mellan 0 och 500.

```csharp
public int GapWidth { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyGapWidthDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Demonstrera GapWidth-egenskapen
            Console.WriteLine("Original GapWidth: " + chart.GapWidth);
            chart.GapWidth = 150; // Set gap width to 150% of default
            Console.WriteLine("Modified GapWidth: " + chart.GapWidth);

            // Spara arbetsboken
            workbook.Save("ChartGapWidthDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


