---
title: "Line.WeightPx"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Line. Obtiene o establece el grosor de la línea en unidades de píxeles"
type: docs
url: /es/net/aspose.cells.drawing/line/weightpx/
---
## Line.WeightPx property

Obtiene o establece el peso de la línea en unidades de píxeles.

```csharp
public double WeightPx { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyWeightPxDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Agregar datos de ejemplo
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            cells["B1"].PutValue(15);
            cells["B2"].PutValue(25);
            cells["B3"].PutValue(35);

            // Agregar un gráfico de líneas
            int chartIndex = workbook.Worksheets[0].Charts.Add(Aspose.Cells.Charts.ChartType.Line, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configura las propiedades de la línea con WeightPx
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Border.WeightPx = 5.0; // Set line weight in pixels
            series.Border.Color = System.Drawing.Color.Blue;

            // Guarda el libro de trabajo
            workbook.Save("LineWeightPxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


