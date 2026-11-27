---
title: "Axis.MaxValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis‑egenskap. Representerar det maximala värdet på värdeaxeln"
type: docs
url: /sv/net/aspose.cells.charts/axis/maxvalue/
---
## Axis.MaxValue property

Anger det maximala värdet på värdeaxeln.

```csharp
public object MaxValue { get; set; }
```

### Anmärkningar

Typen för maxValue kan endast vara double eller DateTime

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMaxValueDemo
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
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(50);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ställ in maxvärdet för värdeaxeln
            chart.ValueAxis.MaxValue = 60;

            // Spara arbetsboken
            workbook.Save("AxisPropertyMaxValueDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


