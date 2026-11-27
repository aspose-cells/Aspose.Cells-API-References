---
title: "GradientStop.Position"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GradientStop property. Positionen för stoppet"
type: docs
url: /sv/net/aspose.cells.drawing/gradientstop/position/
---
## GradientStop.Position property

Positionen för stoppet.

```csharp
public double Position { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class GradientStopPropertyPositionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // Konfigurera gradientfyllning för den första serien
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.Gradient;
            series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
                Aspose.Cells.Drawing.PresetThemeGradientType.RadialGradient, 
                ThemeColorType.Accent1);

            // Åtkomst till och ändra gradientstoppens positioner
            GradientStopCollection stops = series.Area.FillFormat.GradientFill.GradientStops;
            stops[0].Position = 0;
            stops[1].Position = 50;
            stops[2].Position = 100;

            // Spara arbetsboken
            workbook.Save("GradientStopPositionDemo.xlsx");
        }
    }
}
```

### Se även

* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


