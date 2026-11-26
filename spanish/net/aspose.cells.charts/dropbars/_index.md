---
title: "Clase DropBars"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Charts.DropBars. Representa las barras superiores e inferiores en un gráfico"
type: docs
url: /es/net/aspose.cells.charts/dropbars/
---
## DropBars class

Representa las barras de subida y bajada en un gráfico.

```csharp
public class DropBars
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Area](../../aspose.cells.charts/dropbars/area/) { get; } | Obtiene el [`Area`](./area/). |
| [Border](../../aspose.cells.charts/dropbars/border/) { get; } | Obtiene el borde [`Line`](../../aspose.cells.drawing/line/). |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class DropBarsDemo
    {
        public static void DropBarsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
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

            // Habilitar barras superiores e inferiores
            chart.NSeries[0].HasUpDownBars = true;

            // Acceder al objeto DropBars
            DropBars upBars = chart.NSeries[0].UpBars;
            DropBars downBars = chart.NSeries[0].DownBars;

            // Personalizar la apariencia de las barras superiores
            upBars.Border.Color = Color.Green;
            upBars.Area.ForegroundColor = Color.LightGreen;

            // Personalizar la apariencia de las barras inferiores
            downBars.Border.Color = Color.Red;
            downBars.Area.ForegroundColor = Color.LightCoral;

            // Guarda el libro de trabajo
            workbook.Save("DropBarsExample.xlsx");
            workbook.Save("DropBarsExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


