---
title: "Enum PresetThemeGradientType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.PresetThemeGradientType enum. Önceden tanımlı tema degrade tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing/presetthemegradienttype/
---
## PresetThemeGradientType enumeration

Ön ayarlı tema degrade tipini temsil eder.

```csharp
public enum PresetThemeGradientType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| LightGradient | `0` | Açık degrade |
| TopSpotlight | `1` | Üst spot ışığı |
| MediumGradient | `2` | Orta degrade |
| BottomSpotlight | `3` | Alt spot ışığı |
| RadialGradient | `4` | Radyal degrade |

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Category 1");
            worksheet.Cells["A3"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // İlk seriye degrade dolgu uygula
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Area.FillFormat.FillType = FillType.Gradient;
            series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
                PresetThemeGradientType.RadialGradient, 
                ThemeColorType.Accent1);

            // Çalışma kitabını kaydedin
            workbook.Save("PresetThemeGradientDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


