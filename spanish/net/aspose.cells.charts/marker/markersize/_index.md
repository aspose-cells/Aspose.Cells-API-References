---
title: "Marker.MarkerSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Marker. Representa el tamaño del marcador en unidades de puntos. Se aplica a gráficos de líneas, gráficos de dispersión o gráficos de radar"
type: docs
url: /es/net/aspose.cells.charts/marker/markersize/
---
## Marker.MarkerSize property

Representa el tamaño del marcador en unidades de puntos. Se aplica a un gráfico de líneas, un gráfico de dispersión o un gráfico de radar.

```csharp
public int MarkerSize { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class MarkerPropertyMarkerSizeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(i + 1);
                worksheet.Cells[i + 1, 1].PutValue((i + 1) * 2);
            }

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregar series - llamada al método corregida
            int seriesIndex = chart.NSeries.Add("B2:B11", true);
            Series series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A11";

            // Establecer propiedades del marcador
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.MarkerSize = 10; // Demonstrating MarkerSize property
            series.Marker.ForegroundColor = Color.Red;
            series.Marker.BackgroundColor = Color.Yellow;

            // Guarda el libro de trabajo
            workbook.Save("MarkerSizeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


