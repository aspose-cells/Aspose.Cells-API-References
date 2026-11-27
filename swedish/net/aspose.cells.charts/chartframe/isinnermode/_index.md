---
title: "ChartFrame.IsInnerMode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartFrame‑egenskap. Anger om storleken på plotområdet inkluderar tick‑markeringar och axelrubriker. False betyder att storleken ska bestämma storleken på plotområdet, tick‑markeringarna och axelrubrikerna"
type: docs
url: /sv/net/aspose.cells.charts/chartframe/isinnermode/
---
## ChartFrame.IsInnerMode property

Anger om storleken på plotområdet inkluderar tick-markeringarna och axelrubrikerna. False anger att storleken ska bestämma storleken på plotområdet, tick-markeringarna och axelrubrikerna.

```csharp
public bool IsInnerMode { get; set; }
```

### Anmärkningar

Endast för Xlsx‑fil.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyIsInnerModeDemo
    {
        public static void Run()
        {
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

            // Lägg till diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Kom åt diagramramen och demonstrera IsInnerMode
            Aspose.Cells.Charts.ChartFrame chartFrame = chart.ChartArea;
            chartFrame.IsInnerMode = true; // Set to use inner mode
            
            // Ställ in några grundläggande egenskaper för att visa effekten
            chartFrame.Border.Color = Color.Blue;
            chartFrame.Border.Style = Aspose.Cells.Drawing.LineType.Solid;
            chartFrame.Area.ForegroundColor = Color.LightYellow;

            workbook.Save("ChartFrameIsInnerModeDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


