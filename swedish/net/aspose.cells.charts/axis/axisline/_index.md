---
title: "Axis.AxisLine"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis-egenskap. Hämtar utseendet på en axel"
type: docs
url: /sv/net/aspose.cells.charts/axis/axisline/
---
## Axis.AxisLine property

Hämtar utseendet för en Axis.

```csharp
public Line AxisLine { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AxisPropertyAxisLineDemo
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

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Åtkomst till värdeaxeln
            Axis valueAxis = chart.ValueAxis;

            // Anpassa axellinjens egenskaper
            valueAxis.AxisLine.Color = Color.Red;
            valueAxis.AxisLine.Style = LineType.DashDot;
            valueAxis.AxisLine.Weight = WeightType.MediumLine;

            // Spara arbetsboken
            workbook.Save("AxisLineDemo.xlsx");
        }
    }
}
```

### Se även

* class [Line](../../../aspose.cells.drawing/line/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


