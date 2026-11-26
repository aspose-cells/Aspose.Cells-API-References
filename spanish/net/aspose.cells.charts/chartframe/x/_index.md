---
title: "ChartFrame.X"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartFrame. Obtiene o establece la coordenada x de la esquina superior izquierda en unidades de 1/4000 del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartframe/x/
---
## ChartFrame.X property

Obtiene o establece la coordenada x de la esquina superior izquierda en unidades de 1/4000 del área del gráfico.

```csharp
[Obsolete("Use ChartFrame.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int X { get; set; }
```

### Observaciones

Cómo convertir unidades de 1/4000 a píxeles? X en píxeles = X * Chart.ChartObject.Width / 4000d;

NOTA: Este miembro está ahora obsoleto. Por favor use la propiedad ChartFrame.XRatioToChart, en su lugar. X = XRatioToChart * 4000. Esta propiedad será eliminada 12 meses después a partir de febrero de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyXDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("X Values");
            sheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
            }

            // Agregar gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Agregar series y establecer valores X/Y
            chart.NSeries.Add("Sheet1!B2:B10", true);
            chart.NSeries[0].XValues = "Sheet1!A2:A10";

            // Agregar línea de tendencia
            chart.NSeries[0].TrendLines.Add(TrendlineType.Linear, "Linear Trend");
            Trendline trendline = chart.NSeries[0].TrendLines[0];
            
            // Configurar etiquetas de datos
            trendline.DataLabels.ShowValue = true;
            trendline.DataLabels.Font.Color = Color.Blue;
            
            // Demostrar el uso de la propiedad X
            trendline.DataLabels.X = -500; // Set X position offset
            trendline.DataLabels.Y = 200;  // Set Y position offset

            // Guarda el libro de trabajo
            workbook.Save("ChartFramePropertyXDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


