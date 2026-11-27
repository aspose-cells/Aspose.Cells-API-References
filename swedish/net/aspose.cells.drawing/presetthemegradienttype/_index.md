---
title: "Enum PresetThemeGradientType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.PresetThemeGradientType enum. Representerar den förinställda temagradienttypen"
type: docs
url: /sv/net/aspose.cells.drawing/presetthemegradienttype/
---
## PresetThemeGradientType enumeration

Representerar den förinställda temagradienttypen.

```csharp
public enum PresetThemeGradientType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| LightGradient | `0` | Ljusgradient |
| TopSpotlight | `1` | Övre spotlight |
| MediumGradient | `2` | Mellangradient |
| BottomSpotlight | `3` | Nedre spotlight |
| RadialGradient | `4` | Radialgradient |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DrawingClassPresetThemeGradientTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Category 1");
            worksheet.Cells["A3"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // Tillämpa gradientfyllning på den första serien
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Area.FillFormat.FillType = FillType.Gradient;
            series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
                PresetThemeGradientType.RadialGradient, 
                ThemeColorType.Accent1);

            // Spara arbetsboken
            workbook.Save("PresetThemeGradientDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


