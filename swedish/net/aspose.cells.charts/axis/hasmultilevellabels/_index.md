---
title: "Axis.HasMultiLevelLabels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis property. Anger om etiketterna ska visas som flernivå"
type: docs
url: /sv/net/aspose.cells.charts/axis/hasmultilevellabels/
---
## Axis.HasMultiLevelLabels property

Indikerar om etiketterna ska visas som flernivå.

```csharp
public bool HasMultiLevelLabels { get; set; }
```

### Anmärkningar

Gäller endast för kategoriaxeln.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyHasMultiLevelLabelsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata med flernivåkategorier
            worksheet.Cells["A1"].PutValue("Main Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Sub Category");
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["B3"].PutValue("Carrot");
            worksheet.Cells["C1"].PutValue("Value");
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(8);
            
            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagrammets dataintervall inklusive flernivåkategorier
            chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "A1:B3";
            
            // Kontrollera och visa HasMultiLevelLabels-egenskapen
            Console.WriteLine("HasMultiLevelLabels: " + chart.CategoryAxis.HasMultiLevelLabels);
            
            // Spara arbetsboken
            workbook.Save("AxisPropertyHasMultiLevelLabelsDemo.xlsx");
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


