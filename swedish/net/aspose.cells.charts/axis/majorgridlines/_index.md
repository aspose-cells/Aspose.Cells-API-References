---
title: "Axis.MajorGridLines"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis‑egenskap. Representerar huvudrutnät på ett diagramaxel"
type: docs
url: /sv/net/aspose.cells.charts/axis/majorgridlines/
---
## Axis.MajorGridLines property

Anger huvudrutnät på ett diagramaxel.

```csharp
public Line MajorGridLines { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AxisPropertyMajorGridLinesDemo
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

            // Konfigurera huvudrutnät
            chart.ValueAxis.MajorGridLines.IsVisible = false;
            chart.CategoryAxis.MajorGridLines.IsVisible = true;
            chart.CategoryAxis.MajorGridLines.Color = Color.Red;

            // Spara arbetsboken
            workbook.Save("AxisPropertyMajorGridLinesDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Line](../../../aspose.cells.drawing/line/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


