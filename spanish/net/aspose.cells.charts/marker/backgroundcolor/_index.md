---
title: "Marker.BackgroundColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Marker. Representa el color de fondo del marcador en un gráfico de líneas, de dispersión o de radar"
type: docs
url: /es/net/aspose.cells.charts/marker/backgroundcolor/
---
## Marker.BackgroundColor property

Representa el color de fondo del marcador en un gráfico de líneas, de dispersión o de radar.

```csharp
public Color BackgroundColor { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MarkerPropertyBackgroundColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);

            // Crear gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.LineWithDataMarkers, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Personalizar la apariencia del marcador
            foreach (Series series in chart.NSeries)
            {
                series.Marker.MarkerStyle = ChartMarkerType.Circle;
                series.Marker.MarkerSize = 12;
                series.Marker.Border.Color = System.Drawing.Color.Blue;
                series.Marker.BackgroundColor = System.Drawing.Color.LightGreen; // Demonstrating BackgroundColor property
            }

            workbook.Save("MarkerBackgroundColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


