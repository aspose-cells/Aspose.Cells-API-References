---
title: "GradientStop.Position"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GradientStop. La posición de la parada"
type: docs
url: /es/net/aspose.cells.drawing/gradientstop/position/
---
## GradientStop.Position property

La posición de la parada.

```csharp
public double Position { get; set; }
```

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);

            // Añade un gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // Configurar relleno degradado para la primera serie
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.Gradient;
            series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
                Aspose.Cells.Drawing.PresetThemeGradientType.RadialGradient, 
                ThemeColorType.Accent1);

            // Acceder y modificar las posiciones de los puntos de parada del degradado
            GradientStopCollection stops = series.Area.FillFormat.GradientFill.GradientStops;
            stops[0].Position = 0;
            stops[1].Position = 50;
            stops[2].Position = 100;

            // Guarda el libro de trabajo
            workbook.Save("GradientStopPositionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [GradientStop](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


