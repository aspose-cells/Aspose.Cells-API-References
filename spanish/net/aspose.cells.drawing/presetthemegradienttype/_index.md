---
title: "Enumeración PresetThemeGradientType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.PresetThemeGradientType enum. Representa el tipo de degradado de tema preestablecido"
type: docs
url: /es/net/aspose.cells.drawing/presetthemegradienttype/
---
## PresetThemeGradientType enumeration

Representa el tipo de degradado de tema preestablecido.

```csharp
public enum PresetThemeGradientType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| LightGradient | `0` | Degradado claro |
| TopSpotlight | `1` | Foco superior |
| MediumGradient | `2` | Degradado medio |
| BottomSpotlight | `3` | Foco inferior |
| RadialGradient | `4` | Degradado radial |

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Category 1");
            worksheet.Cells["A3"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // Aplicar relleno de degradado a la primera serie
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Area.FillFormat.FillType = FillType.Gradient;
            series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
                PresetThemeGradientType.RadialGradient, 
                ThemeColorType.Accent1);

            // Guarda el libro de trabajo
            workbook.Save("PresetThemeGradientDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


