---
title: "Line.ThemeColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Line-egenskap. Hämtar och anger temafärgen"
type: docs
url: /sv/net/aspose.cells.drawing/line/themecolor/
---
## Line.ThemeColor property

Hämtar och anger temafärgen.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Anmärkningar

Om förgrundsfärgen inte är en temafärg returneras NULL.

### Exempel

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyThemeColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Series 1");
            sheet.Cells["C1"].PutValue("Series 2");
            
            for (int i = 2; i <= 6; i++)
            {
                sheet.Cells["A" + i].PutValue("Cat " + (i-1));
                sheet.Cells["B" + i].PutValue(i * 10);
                sheet.Cells["C" + i].PutValue(i * 15);
            }

            // Lägg till ett linjediagram
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.SetChartDataRange("B1:C6", true);
            chart.NSeries.CategoryData = "A2:A6";

            // Anpassa seriens utseende med ThemeColor
            var seriesThemes = new List<ThemeColorType> { 
                ThemeColorType.Accent1, 
                ThemeColorType.Accent2 
            };

            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                chart.NSeries[i].Border.ThemeColor = new ThemeColor(seriesThemes[i], 0.6);
                chart.NSeries[i].Border.Style = LineType.Solid;
                chart.NSeries[i].Border.Weight = WeightType.MediumLine;
            }

            // Spara arbetsboken
            workbook.Save("LineChartWithThemeColor.xlsx");
        }
    }
}
```

### Se även

* class [ThemeColor](../../../aspose.cells/themecolor/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


