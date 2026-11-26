---
title: "Clase Marker"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.Marker class. Representa el marcador en un gráfico de líneas, de dispersión o de radar"
type: docs
url: /es/net/aspose.cells.charts/marker/
---
## Marker class

Representa el marcador en un gráfico de líneas, de dispersión o de radar.

```csharp
public class Marker
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Area](../../aspose.cells.charts/marker/area/) { get; } | Obtiene el [`area`](./area/). |
| [BackgroundColor](../../aspose.cells.charts/marker/backgroundcolor/) { get; set; } | Representa el color de fondo del marcador en un gráfico de líneas, de dispersión o de radar. |
| [BackgroundColorSetType](../../aspose.cells.charts/marker/backgroundcolorsettype/) { get; set; } | Obtiene o establece el tipo de conjunto de color de fondo del marcador. |
| [Border](../../aspose.cells.charts/marker/border/) { get; } | Obtiene el [`border`](../../aspose.cells.drawing/line/). |
| [ForegroundColor](../../aspose.cells.charts/marker/foregroundcolor/) { get; set; } | Representa el color de primer plano del marcador en un gráfico de líneas, de dispersión o de radar. |
| [ForegroundColorSetType](../../aspose.cells.charts/marker/foregroundcolorsettype/) { get; set; } | Obtiene o establece el tipo de conjunto de color de primer plano del marcador. |
| [MarkerSize](../../aspose.cells.charts/marker/markersize/) { get; set; } | Representa el tamaño del marcador en unidades de puntos. Se aplica a un gráfico de líneas, un gráfico de dispersión o un gráfico de radar. |
| [MarkerSizePx](../../aspose.cells.charts/marker/markersizepx/) { get; set; } | Representa el tamaño del marcador en unidades de píxeles. Se aplica a gráficos de líneas, gráficos de dispersión o gráficos de radar. |
| [MarkerStyle](../../aspose.cells.charts/marker/markerstyle/) { get; set; } | Representa el estilo del marcador. Se aplica a un gráfico de líneas, un gráfico de dispersión o un gráfico de radar. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MarkerDemo
    {
        public static void MarkerExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            // Obtenga la referencia de la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Agrega NSeries (fuente de datos del gráfico) al gráfico que abarca desde la celda "A1" hasta "B3"
            chart.NSeries.Add("A1:B3", true);

            // Acceder a la primera serie
            Series series = chart.NSeries[0];

            // Establecer propiedades del marcador
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.MarkerSize = 10; // Size in points
            series.Marker.MarkerSizePx = 20; // Size in pixels
            series.Marker.ForegroundColor = Color.Red;
            series.Marker.ForegroundColorSetType = FormattingType.Custom;
            series.Marker.BackgroundColor = Color.Yellow;
            series.Marker.BackgroundColorSetType = FormattingType.Custom;

            // Guarda el libro de trabajo
            workbook.Save("MarkerExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


