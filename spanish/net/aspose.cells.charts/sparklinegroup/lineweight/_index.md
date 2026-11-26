---
title: "SparklineGroup.LineWeight"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineGroup. Obtiene y establece el grosor de línea en cada sparkline de línea del grupo de sparklines en unidades de puntos"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/lineweight/
---
## SparklineGroup.LineWeight property

Obtiene y establece el grosor de línea en cada sparkline de línea del grupo de sparkline, en unidades de puntos.

```csharp
public double LineWeight { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyLineWeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Datos de ejemplo
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Crear grupo de sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Establecer la propiedad LineWeight
            group.LineWeight = 2.5; // Thicker line weight for visibility

            workbook.Save("SparklineLineWeightDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


