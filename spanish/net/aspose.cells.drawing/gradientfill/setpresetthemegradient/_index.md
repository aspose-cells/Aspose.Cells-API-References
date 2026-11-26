---
title: "GradientFill.SetPresetThemeGradient"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GradientFill. Establece el relleno de degradado de tema preestablecido"
type: docs
url: /es/net/aspose.cells.drawing/gradientfill/setpresetthemegradient/
---
## GradientFill.SetPresetThemeGradient method

Establece el relleno degradado de tema preestablecido.

```csharp
public void SetPresetThemeGradient(PresetThemeGradientType gradientType, 
    ThemeColorType themeColorType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| gradientType | PresetThemeGradientType | El tipo de degradado preestablecido. |
| themeColorType | ThemeColorType | El tipo de color del tema. |

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Sample");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.SetChartDataRange("A1:A4", false);

            // Configurar el relleno de la serie con degradado
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.Gradient;
            
            // Demostrar SetPresetThemeGradient con parámetros especificados
            series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
                Aspose.Cells.Drawing.PresetThemeGradientType.RadialGradient, 
                Aspose.Cells.ThemeColorType.Accent1);

            // Guarda el libro de trabajo
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PresetThemeGradientType](../../presetthemegradienttype/)
* enum [ThemeColorType](../../../aspose.cells/themecolortype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


