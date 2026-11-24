---
title: "Enum PresetThemeGradientType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.PresetThemeGradientType Enum. Stellt den voreingestellten Themenverlauftyp dar"
type: docs
url: /de/net/aspose.cells.drawing/presetthemegradienttype/
---
## PresetThemeGradientType enumeration

Stellt den voreingestellten Themen‑Gradient‑Typ dar.

```csharp
public enum PresetThemeGradientType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| LightGradient | `0` | Heller Verlauf |
| TopSpotlight | `1` | Oberes Spotlicht |
| MediumGradient | `2` | Mittlerer Verlauf |
| BottomSpotlight | `3` | Unteres Spotlicht |
| RadialGradient | `4` | Radialer Verlauf |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Category 1");
            worksheet.Cells["A3"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // Verlauffüllung auf die erste Serie anwenden
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Area.FillFormat.FillType = FillType.Gradient;
            series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
                PresetThemeGradientType.RadialGradient, 
                ThemeColorType.Accent1);

            // Speichere die Arbeitsmappe
            workbook.Save("PresetThemeGradientDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


