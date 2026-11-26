---
title: "SparklineGroup.FirstPointColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineGroup. Obtiene y establece el color del primer punto de datos en el grupo de sparklines"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/firstpointcolor/
---
## SparklineGroup.FirstPointColor property

Obtiene y establece el color del primer punto de datos en el grupo de sparkline.

```csharp
public CellsColor FirstPointColor { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyFirstPointColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["A2"].PutValue(3);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(4);

            // Crear grupo de sparkline
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 3;
            ca.StartColumn = 1;
            ca.EndColumn = 1;
            
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:A4", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Establecer FirstPointColor
            group.ShowFirstPoint = true;
            CellsColor firstPointColor = workbook.CreateCellsColor();
            firstPointColor.Color = Color.Purple;
            group.FirstPointColor = firstPointColor;

            // Guarda el libro de trabajo
            workbook.Save("SparklineFirstPointColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


