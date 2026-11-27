---
title: "ChartFrame.Area"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame‑egenskap. Hämtar området"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/area/
---
## ChartFrame.Area property

Hämtar `area`.

```csharp
public virtual Area Area { get; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyAreaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Åtkomst till diagramområdet
            ChartArea chartArea = chart.ChartArea;
            
            // Demonstrera funktionaliteten för Area‑egenskapen
            Area area = chartArea.Area;
            Console.WriteLine("Original Formatting: " + area.Formatting);
            
            // Modifiera areaegenskaper
            area.Formatting = FormattingType.Custom;
            area.BackgroundColor = Color.LightBlue;
            area.ForegroundColor = Color.DarkBlue;
            area.Transparency = 0.3;
            area.InvertIfNegative = true;

            // Spara arbetsboken
            workbook.Save("ChartFramePropertyAreaDemo.xlsx");
        }
    }
}
```

### Se även

* class [Area](../../../aspose.cells.drawing/area/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


