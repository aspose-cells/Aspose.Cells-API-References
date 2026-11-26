---
title: "Chart.PlotVisibleCells"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del gráfico. Indica si solo se trazan celdas visibles"
type: docs
url: /es/net/aspose.cells.charts/chart/plotvisiblecells/
---
## Chart.PlotVisibleCells property

Indica si solo se trazan celdas visibles.

```csharp
[Obsolete("Use PlotVisibleCellsOnly property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool PlotVisibleCells { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad PlotVisibleCellsOnly. Este método será eliminado 12 meses después, desde diciembre de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotVisibleCellsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("Alice");
            worksheet.Cells["A3"].PutValue("Bob");
            worksheet.Cells["A4"].PutValue("Eve");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(90);
            worksheet.Cells["B3"].PutValue(85);
            worksheet.Cells["B4"].PutValue(95);

            // Ocultar algunas filas
            worksheet.Cells.HideRow(2);
            worksheet.Cells.HideRow(3);

            // Crear gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Demostrar la propiedad PlotVisibleCells
            chart.PlotVisibleCells = false; // Will not plot hidden cells
            // chart.PlotVisibleCells = true; // Graficará celdas ocultas (comentado para la demostración)

            // Guarda el libro de trabajo
            workbook.Save("ChartPlotVisibleCellsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


