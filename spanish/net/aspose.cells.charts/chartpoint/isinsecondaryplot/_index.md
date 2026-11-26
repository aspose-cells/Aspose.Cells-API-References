---
title: "ChartPoint.IsInSecondaryPlot"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ChartPoint. Obtiene o establece un valor que indica si este punto de datos está en el segundo pastel o barra en un gráfico de pastel dentro de pastel o barra dentro de pastel."
type: docs
url: /es/net/aspose.cells.charts/chartpoint/isinsecondaryplot/
---
## ChartPoint.IsInSecondaryPlot property

Obtiene o establece un valor que indica si este punto de datos está en el segundo pastel o barra en un gráfico de pie of pie o bar of pie.

```csharp
public bool IsInSecondaryPlot { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyIsInSecondaryPlotDemo
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

            // Crear un gráfico de pastel que admita trazados secundarios
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configurar el trazado secundario
            chart.NSeries[0].Points[2].IsInSecondaryPlot = true;
            chart.NSeries[0].Points[3].IsInSecondaryPlot = true;

            // Guardar la salida
            workbook.Save("PieChartWithSecondaryPlot.xlsx");
        }
    }
}
```

### Ver también

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


