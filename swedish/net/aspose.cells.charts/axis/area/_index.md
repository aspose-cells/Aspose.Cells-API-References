---
title: "Axis.Area"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis-egenskap. Hämtar området"
type: docs
url: /sv/net/aspose.cells.charts/axis/area/
---
## Axis.Area property

Hämtar `Area`.

```csharp
public Area Area { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AxisPropertyAreaDemo
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
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Åtkomst till egenskaper för kategoriekaxelns område
            chart.CategoryAxis.Area.BackgroundColor = Color.LightBlue;
            chart.CategoryAxis.Area.ForegroundColor = Color.White;
            chart.CategoryAxis.Area.Formatting = FormattingType.Custom;
            
            // Spara arbetsboken
            workbook.Save("AxisPropertyAreaDemo_Output.xlsx");
            
            Console.WriteLine("Category Axis Area Background Color: " + chart.CategoryAxis.Area.BackgroundColor);
        }
    }
}
```

### Se även

* class [Area](../../../aspose.cells.drawing/area/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


