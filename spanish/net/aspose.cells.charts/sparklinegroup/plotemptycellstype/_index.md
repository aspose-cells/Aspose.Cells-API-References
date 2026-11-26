---
title: "SparklineGroup.PlotEmptyCellsType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineGroup. Indica cómo trazar celdas vacías"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/plotemptycellstype/
---
## SparklineGroup.PlotEmptyCellsType property

Indica cómo trazar celdas vacías.

```csharp
public PlotEmptyCellsType PlotEmptyCellsType { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyPlotEmptyCellsTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos con algunas celdas vacías
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(null); // Empty cell
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Define el CellArea para el sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Agregar un grupo de sparkline
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Establecer cómo deben trazarse las celdas vacías
            group.PlotEmptyCellsType = PlotEmptyCellsType.Zero;

            // Agregar sparkline al grupo
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Guarda el libro de trabajo
            workbook.Save("SparklineEmptyCellsDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PlotEmptyCellsType](../../plotemptycellstype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


