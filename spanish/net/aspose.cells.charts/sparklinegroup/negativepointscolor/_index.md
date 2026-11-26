---
title: "SparklineGroup.NegativePointsColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineGroup. Obtiene y establece el color de los valores negativos en el grupo de sparkline"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/negativepointscolor/
---
## SparklineGroup.NegativePointsColor property

Obtiene y establece el color de los valores negativos en el grupo de sparkline.

```csharp
public CellsColor NegativePointsColor { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyNegativePointsColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos con valores negativos para demostrar puntos negativos
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(-2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(-3);

            // Define el CellArea para el sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Agregar grupo de sparkline
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Configurar el color de los puntos negativos
            group.ShowNegativePoints = true;
            CellsColor negativePointsColor = workbook.CreateCellsColor();
            negativePointsColor.Color = Color.Blue;
            group.NegativePointsColor = negativePointsColor;

            workbook.Save("SparklineNegativePointsColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


