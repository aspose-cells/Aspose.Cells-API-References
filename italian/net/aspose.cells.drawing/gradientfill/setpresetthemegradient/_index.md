---
title: "GradientFill.SetPresetThemeGradient"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo GradientFill. Imposta il riempimento gradiente del tema predefinito"
type: docs
url: /it/net/aspose.cells.drawing/gradientfill/setpresetthemegradient/
---
## GradientFill.SetPresetThemeGradient method

Imposta il riempimento a gradiente predefinito del tema.

```csharp
public void SetPresetThemeGradient(PresetThemeGradientType gradientType, 
    ThemeColorType themeColorType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| gradientType | PresetThemeGradientType | Il tipo di gradiente predefinito. |
| themeColorType | ThemeColorType | Il tipo di colore del tema. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Sample");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:A4", false);

            // Configura il riempimento della serie con gradiente
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.Gradient;
            
            // Dimostra SetPresetThemeGradient con i parametri specificati
            series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
                Aspose.Cells.Drawing.PresetThemeGradientType.RadialGradient, 
                Aspose.Cells.ThemeColorType.Accent1);

            // Salva la cartella di lavoro
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PresetThemeGradientType](../../presetthemegradienttype/)
* enum [ThemeColorType](../../../aspose.cells/themecolortype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


