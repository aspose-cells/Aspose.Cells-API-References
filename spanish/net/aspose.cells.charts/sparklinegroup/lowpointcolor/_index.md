---
title: "SparklineGroup.LowPointColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineGroup. Obtiene y establece el color de los puntos más bajos de los datos en el grupo de sparkline"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/lowpointcolor/
---
## SparklineGroup.LowPointColor property

Obtiene y establece el color de los puntos más bajos de datos en el grupo de sparkline.

```csharp
public CellsColor LowPointColor { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyLowPointColorDemo
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
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Agregar grupo de sparkline usando la API correcta
            int idx = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[idx];
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Personalizar la apariencia del sparkline
            group.ShowLowPoint = true;
            group.LowPointColor.Color = Color.Red;

            workbook.Save("SparklineLowPointColorDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


