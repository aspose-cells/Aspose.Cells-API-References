---
title: "SparklineGroup.ShowHighPoint"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineGroup. Indica si se deben resaltar los puntos más altos de los datos en el grupo de sparkline."
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/showhighpoint/
---
## SparklineGroup.ShowHighPoint property

Indica si se debe resaltar los puntos más altos de datos en el grupo de sparkline.

```csharp
public bool ShowHighPoint { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowHighPointDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datos de ejemplo
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Crear grupo de sparkline
            CellArea cellArea = new CellArea { StartColumn = 4, EndColumn = 4, StartRow = 0, EndRow = 0 };
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];

            // Agregar sparkline
            group.Sparklines.Add("A1:D1", 0, 4);

            // Configurar la visualización del punto alto
            group.ShowHighPoint = true;
            CellsColor highColor = workbook.CreateCellsColor();
            highColor.Color = System.Drawing.Color.Green;
            group.HighPointColor = highColor;

            // Guardar el libro de trabajo
            workbook.Save("SparklineHighPointDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


