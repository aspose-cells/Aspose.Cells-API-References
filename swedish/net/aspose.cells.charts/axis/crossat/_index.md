---
title: "Axis.CrossAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis-egenskap. Representerar punkten på värdeaxeln där kategoriaxeln korsar den"
type: docs
url: /sv/net/aspose.cells.charts/axis/crossat/
---
## Axis.CrossAt property

Representerar punkten på värdeaxeln där kategoriaxeln korsar den.

```csharp
public double CrossAt { get; set; }
```

### Anmärkningar

Numret bör vara ett heltal när det gäller kategoriaxeln. Och värdet måste vara mellan 1 och 31999.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyCrossAtDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Konfigurera värdeaxeln
            chart.ValueAxis.CrossAt = 15; // Cross at value 15
            chart.ValueAxis.MinValue = 0;
            chart.ValueAxis.MaxValue = 50;

            // Konfigurera kategoriaxeln
            chart.CategoryAxis.CrossAt = 2.5; // Cross between categories B and C
            chart.CategoryAxis.TickLabelPosition = Aspose.Cells.Charts.TickLabelPositionType.Low;

            // Spara arbetsboken
            workbook.Save("AxisCrossAtDemo.xlsx");
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


