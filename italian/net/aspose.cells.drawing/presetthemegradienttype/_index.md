---
title: "Enum PresetThemeGradientType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.PresetThemeGradientType enum. Rappresenta il tipo di gradiente tema predefinito"
type: docs
url: /it/net/aspose.cells.drawing/presetthemegradienttype/
---
## PresetThemeGradientType enumeration

Rappresenta il tipo di gradiente tematico predefinito.

```csharp
public enum PresetThemeGradientType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| LightGradient | `0` | Gradiente chiaro |
| TopSpotlight | `1` | Spotlight superiore |
| MediumGradient | `2` | Gradiente medio |
| BottomSpotlight | `3` | Spotlight inferiore |
| RadialGradient | `4` | Gradiente radiale |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Category 1");
            worksheet.Cells["A3"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // Applica riempimento a gradiente alla prima serie
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Area.FillFormat.FillType = FillType.Gradient;
            series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
                PresetThemeGradientType.RadialGradient, 
                ThemeColorType.Accent1);

            // Salva la cartella di lavoro
            workbook.Save("PresetThemeGradientDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


