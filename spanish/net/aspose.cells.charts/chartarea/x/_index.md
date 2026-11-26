---
title: "ChartArea.X"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartArea. Obtiene o establece el desplazamiento horizontal desde la columna de su esquina superior izquierda en unidades de 1/4000 del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartarea/x/
---
## ChartArea.X property

Obtiene o establece el desplazamiento horizontal desde la columna de su esquina superior izquierda, en unidades de 1/4000 del área del gráfico.

```csharp
[Obsolete("Use ChartArea.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int X { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. Por favor, use la propiedad ChartArea.XRatioToChart, en su lugar. X = XRatioToChart * 4000. Esta propiedad será eliminada 12 meses después desde febrero de 2025. Aspose se disculpa por cualquier inconveniente que pueda haber experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyXDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configure el área del gráfico
            Aspose.Cells.Charts.ChartArea chartArea = chart.ChartArea;
            chartArea.X = 10; // Demonstrating X property usage
            chartArea.Y = 10;
            chartArea.Width = 400;
            chartArea.Height = 300;

            // Guardar salida
            workbook.Save("ChartAreaXDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


