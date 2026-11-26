---
title: "SparklineGroup.SeriesColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineGroup. Obtiene y establece el color de los sparklines en el grupo de sparklines"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/seriescolor/
---
## SparklineGroup.SeriesColor property

Obtiene y establece el color de los sparklines en el grupo de sparkline.

```csharp
public CellsColor SeriesColor { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertySeriesColorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Datos de ejemplo
            ws.Cells["A1"].PutValue(5);
            ws.Cells["A2"].PutValue(8);
            ws.Cells["A3"].PutValue(3);
            
            // Crear grupo de sparkline
            CellArea dataRange = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            CellArea locationRange = new CellArea { StartRow = 0, EndRow = 0, StartColumn = 1, EndColumn = 1 };
            int index = ws.SparklineGroups.Add(SparklineType.Column, "A1:A3", false, locationRange);
            
            // Establecer color de la serie
            SparklineGroup group = ws.SparklineGroups[index];
            CellsColor color = wb.CreateCellsColor();
            color.Color = Color.Blue;
            group.SeriesColor = color;
            
            wb.Save("SparklineSeriesColorDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


