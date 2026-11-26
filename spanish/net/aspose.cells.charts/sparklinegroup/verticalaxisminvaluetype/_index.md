---
title: "SparklineGroup.VerticalAxisMinValueType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineGroup. Representa el tipo de valor mínimo del eje vertical."
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/verticalaxisminvaluetype/
---
## SparklineGroup.VerticalAxisMinValueType property

Representa el tipo de valor mínimo del eje vertical.

```csharp
public SparklineAxisMinMaxType VerticalAxisMinValueType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyVerticalAxisMinValueTypeDemo
    {
        public static void Run()
        {
            // Crea un libro de trabajo y una hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Definir la ubicación del sparkline
            CellArea cellArea = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Agregar grupo de sparkline
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Establecer el tipo de valor mínimo del eje vertical
            group.VerticalAxisMinValueType = SparklineAxisMinMaxType.AutoIndividual;

            // Guarda el libro de trabajo
            workbook.Save("SparklineVerticalAxisMinValueTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [SparklineAxisMinMaxType](../../sparklineaxisminmaxtype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


