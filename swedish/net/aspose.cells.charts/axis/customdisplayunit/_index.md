---
title: "Axis.CustomDisplayUnit"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis-egenskap. Anger ett anpassat värde för visningsenheten"
type: docs
url: /sv/net/aspose.cells.charts/axis/customdisplayunit/
---
## Axis.CustomDisplayUnit property

Anger ett anpassat värde för visningsenheten.

```csharp
public double CustomDisplayUnit { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyCustomDisplayUnitDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10000000);
            worksheet.Cells["B3"].PutValue(20000000);
            worksheet.Cells["B4"].PutValue(30000000);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Ställ in anpassad visningsenhet för värdeaxeln
            chart.ValueAxis.CustomDisplayUnit = 1.0E7;
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Custom;
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


