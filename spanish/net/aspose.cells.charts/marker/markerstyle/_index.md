---
title: "Marker.MarkerStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Marker. Representa el estilo del marcador. Se aplica a un gráfico de líneas, un gráfico de dispersión o un gráfico de radar"
type: docs
url: /es/net/aspose.cells.charts/marker/markerstyle/
---
## Marker.MarkerStyle property

Representa el estilo del marcador. Se aplica a un gráfico de líneas, un gráfico de dispersión o un gráfico de radar.

```csharp
public ChartMarkerType MarkerStyle { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MarkerPropertyMarkerStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["B2"].PutValue(4);
            sheet.Cells["B3"].PutValue(5);
            sheet.Cells["B4"].PutValue(6);

            // Añade un gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Establecer origen de datos del Chart
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "B2:B4";

            // Establecer el estilo del marcador para la primera serie
            chart.NSeries[0].Marker.MarkerStyle = ChartMarkerType.Circle;
            chart.NSeries[0].Marker.ForegroundColor = System.Drawing.Color.Blue;
            chart.NSeries[0].Marker.BackgroundColor = System.Drawing.Color.White;
            chart.NSeries[0].Marker.MarkerSize = 10;

            // Guarda el libro de trabajo
            workbook.Save("MarkerStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ChartMarkerType](../../chartmarkertype/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


