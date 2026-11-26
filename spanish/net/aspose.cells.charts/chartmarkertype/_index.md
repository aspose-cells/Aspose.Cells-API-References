---
title: "Enumeración ChartMarkerType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Charts.ChartMarkerType. Representa el estilo de marcador en un gráfico de líneas, gráfico de dispersión o gráfico de radar"
type: docs
url: /es/net/aspose.cells.charts/chartmarkertype/
---
## ChartMarkerType enumeration

Representa el estilo del marcador en un gráfico de líneas, de dispersión o de radar.

```csharp
public enum ChartMarkerType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Automatic | `0` | Marcadores automáticos. |
| Circle | `1` | Marcadores circulares. |
| Dash | `2` | Marcadores de barra larga |
| Diamond | `3` | Marcadores en forma de diamante. |
| Dot | `4` | Marcadores de barra corta. |
| None | `5` | Sin marcadores. |
| SquarePlus | `6` | Marcadores cuadrados con un signo más. |
| Square | `7` | Marcadores cuadrados. |
| SquareStar | `8` | Marcadores cuadrados con un asterisco. |
| Triangle | `9` | Marcadores triangulares. |
| SquareX | `10` | Marcadores cuadrados con una X. |
| Picture | `11` | Imagen |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartMarkerTypeDemo
    {
        public static void ChartMarkerTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregar la serie de datos al gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder al marcador de la primera serie
            Marker marker = chart.NSeries[0].Marker;

            // Establecer el estilo del marcador
            marker.MarkerStyle = ChartMarkerType.Circle;

            // Establecer el tamaño del marcador
            marker.MarkerSize = 10;

            // Establecer los colores de primer plano y de fondo del marcador
            marker.ForegroundColor = Color.Red;
            marker.BackgroundColor = Color.Yellow;

            // Guarda el libro de trabajo
            workbook.Save("ChartMarkerTypeExample.xlsx");
            workbook.Save("ChartMarkerTypeExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


