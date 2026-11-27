---
title: "GradientFill.SetPresetThemeGradient"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GradientFill-metod. Ställer in förinställd temagradientfyllning"
type: docs
url: /sv/net/aspose.cells.drawing/gradientfill/setpresetthemegradient/
---
## GradientFill.SetPresetThemeGradient method

Ställer in förinställd temagradientfyllning.

```csharp
public void SetPresetThemeGradient(PresetThemeGradientType gradientType, 
    ThemeColorType themeColorType)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| gradientType | PresetThemeGradientType | Den förinställda gradienttypen. |
| themeColorType | ThemeColorType | Temafärgstypen. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillMethodSetPresetThemeGradientWithPresetThemeGradientTypeThemeCoDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Sample");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.SetChartDataRange("A1:A4", false);

            // Konfigurera seriefyllning med gradient
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.Gradient;
            
            // Demonstrera SetPresetThemeGradient med angivna parametrar
            series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
                Aspose.Cells.Drawing.PresetThemeGradientType.RadialGradient, 
                Aspose.Cells.ThemeColorType.Accent1);

            // Spara arbetsboken
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PresetThemeGradientType](../../presetthemegradienttype/)
* enum [ThemeColorType](../../../aspose.cells/themecolortype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


