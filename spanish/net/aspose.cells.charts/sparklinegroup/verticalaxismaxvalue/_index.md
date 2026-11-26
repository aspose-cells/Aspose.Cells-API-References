---
title: "SparklineGroup.VerticalAxisMaxValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineGroup. Obtiene y establece el valor máximo personalizado para el eje vertical"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/verticalaxismaxvalue/
---
## SparklineGroup.VerticalAxisMaxValue property

Obtiene y establece el valor máximo personalizado para el eje vertical.

```csharp
public double VerticalAxisMaxValue { get; set; }
```

### Observaciones

Si esta propiedad está establecida, [`VerticalAxisMaxValueType`](../verticalaxismaxvaluetype/) será Custom.

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyVerticalAxisMaxValueDemo
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

            // Definir la ubicación del sparkline
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

            // Agregar sparkline
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Establecer el valor máximo del eje vertical
            group.VerticalAxisMaxValueType = SparklineAxisMinMaxType.Custom;
            group.VerticalAxisMaxValue = 10.0;

            // Guarda el libro de trabajo
            workbook.Save("SparklineVerticalAxisMaxValueDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


