---
title: "Chart.Style"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart egenskap. Hämtar och anger den inbyggda stilen"
type: docs
url: /sv/net/aspose.cells.charts/chart/style/
---
## Chart.Style property

Hämtar och anger den inbyggda stilen.

```csharp
public int Style { get; set; }
```

### Anmärkningar

Den bör vara mellan 1 och 48. Returnera -1 om den inte är inställd.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart1 = worksheet.Charts[chartIndex];
            chart1.NSeries.Add("B2:B4", false);
            chart1.NSeries.CategoryData = "A2:A4";

            // Skapa ett annat diagram och kopiera stilen från det första diagrammet
            chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 10, 20, 18);
            Aspose.Cells.Charts.Chart chart2 = worksheet.Charts[chartIndex];
            chart2.NSeries.Add("B2:B4", false);
            chart2.NSeries.CategoryData = "A2:A4";
            
            // Demonstrera användning av Style-egenskapen
            chart2.Style = chart1.Style;

            // Spara arbetsboken
            workbook.Save("ChartStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


