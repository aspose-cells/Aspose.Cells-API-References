---
title: "SparklineGroup.PlotRightToLeft"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineGroup. Indica si los datos del gráfico se trazan de derecha a izquierda"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/plotrighttoleft/
---
## SparklineGroup.PlotRightToLeft property

Indica si los datos del gráfico se presentan de derecha a izquierda.

```csharp
public bool PlotRightToLeft { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyPlotRightToLeftDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Crear grupo de sparkline
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Agregar sparkline
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Establecer colores de sparkline
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Orange;
            group.SeriesColor = seriesColor;

            // Demostrar la propiedad PlotRightToLeft
            group.PlotRightToLeft = true; // Plot data points from right to left

            // Guarda el libro de trabajo
            workbook.Save("SparklineRightToLeftDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


