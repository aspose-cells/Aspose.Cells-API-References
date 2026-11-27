---
title: "ChartFrame.IsAutomaticSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame-egenskap. Anger om diagramramen har automatisk storlek"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/isautomaticsize/
---
## ChartFrame.IsAutomaticSize property

Anger om diagramramen har automatisk storlek.

```csharp
public virtual bool IsAutomaticSize { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyIsAutomaticSizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Få åtkomst till legend och demonstrera IsAutomaticSize‑egenskapen
            Aspose.Cells.Charts.Legend legend = chart.Legend;
            
            // Ställ in automatisk storlek till falskt och visa värdet
            legend.IsAutomaticSize = false;
            Console.WriteLine("Legend Automatic Size: " + legend.IsAutomaticSize);
            
            // Ställ in automatisk storlek till sant och visa värdet
            legend.IsAutomaticSize = true;
            Console.WriteLine("Legend Automatic Size: " + legend.IsAutomaticSize);
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


