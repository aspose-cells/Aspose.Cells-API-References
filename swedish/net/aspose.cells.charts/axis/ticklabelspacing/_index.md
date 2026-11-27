---
title: "Axis.TickLabelSpacing"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis-egenskap. Representerar antalet kategorier eller serier mellan tickmark-etiketter. Gäller endast för kategori- och serieaxlar"
type: docs
url: /sv/net/aspose.cells.charts/axis/ticklabelspacing/
---
## Axis.TickLabelSpacing property

Anger antalet kategorier eller serier mellan tick‑etiketter. Gäller endast för kategori‑ och serieaxlar.

```csharp
public int TickLabelSpacing { get; set; }
```

### Anmärkningar

Numret måste vara mellan 1 och 31999.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTickLabelSpacingDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B5"].PutValue(40);

            // Lägg till diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagramdata
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Konfigurera avståndet mellan axelns tick-etiketter
            chart.CategoryAxis.TickLabelSpacing = 2; // Show every 2nd label

            workbook.Save("AxisPropertyTickLabelSpacingDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


