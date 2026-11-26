---
title: "SparklineGroup.ShowNegativePoints"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineGroup. Indica si se deben resaltar los valores negativos en el grupo de sparkline con un color o marcador diferente."
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/shownegativepoints/
---
## SparklineGroup.ShowNegativePoints property

Indica si se deben resaltar los valores negativos en el grupo de sparkline con un color o marcador diferente.

```csharp
public bool ShowNegativePoints { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowNegativePointsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos con valores negativos para demostrar ShowNegativePoints
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

            // Agregar un grupo de sparkline
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Configurar las propiedades del grupo de sparkline
            group.ShowNegativePoints = true;
            CellsColor negativePointsColor = workbook.CreateCellsColor();
            negativePointsColor.Color = Color.Blue;
            group.NegativePointsColor = negativePointsColor;

            // Guarda el libro de trabajo
            workbook.Save("SparklineNegativePointsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


