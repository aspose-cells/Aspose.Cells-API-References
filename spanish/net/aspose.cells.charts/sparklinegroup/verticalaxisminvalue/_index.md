---
title: "SparklineGroup.VerticalAxisMinValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineGroup. Obtiene y establece el valor mínimo personalizado para el eje vertical."
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/verticalaxisminvalue/
---
## SparklineGroup.VerticalAxisMinValue property

Obtiene y establece el valor mínimo personalizado para el eje vertical.

```csharp
public double VerticalAxisMinValue { get; set; }
```

### Observaciones

Si esta propiedad está establecida, [`VerticalAxisMinValueType`](../verticalaxisminvaluetype/) será Custom.

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyVerticalAxisMinValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["A2"].PutValue(2);
            sheet.Cells["A3"].PutValue(1);
            sheet.Cells["A4"].PutValue(3);

            // Crear grupo de sparkline
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 3;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:A4", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Establecer el valor mínimo del eje vertical
            group.VerticalAxisMinValueType = SparklineAxisMinMaxType.Custom;
            group.VerticalAxisMinValue = 0.0;

            // Guarda el libro de trabajo
            workbook.Save("SparklineVerticalAxisMinValueDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


