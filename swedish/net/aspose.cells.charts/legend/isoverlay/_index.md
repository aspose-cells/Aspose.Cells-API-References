---
title: "Legend.IsOverLay"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Legend-egenskap. Hämtar eller anger om legenden ska visas utan att överlappa diagrammet"
type: docs
url: /sv/net/aspose.cells.charts/legend/isoverlay/
---
## Legend.IsOverLay property

Hämtar eller anger om förklaringen ska visas utan att överlappa diagrammet.

```csharp
public bool IsOverLay { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendPropertyIsOverLayDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
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
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Ställ in legendöverlappning
            chart.Legend.IsOverLay = true;
            
            // Spara arbetsboken
            workbook.Save("LegendOverlayDemo.xlsx");
            
            Console.WriteLine("Chart with overlay legend created successfully.");
        }
    }
}
```

### Se även

* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


