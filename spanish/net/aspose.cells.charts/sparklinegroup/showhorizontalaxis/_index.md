---
title: "SparklineGroup.ShowHorizontalAxis"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineGroup. Indica si se debe mostrar el eje horizontal del sparkline. El eje horizontal aparece si el sparkline tiene datos que cruzan el eje cero"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/showhorizontalaxis/
---
## SparklineGroup.ShowHorizontalAxis property

Indica si se debe mostrar el eje horizontal del sparkline. El eje horizontal aparece si el sparkline tiene datos que cruzan el eje cero.

```csharp
public bool ShowHorizontalAxis { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowHorizontalAxisDemo
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

            // Configurar propiedades de sparkline
            group.ShowHorizontalAxis = true;
            CellsColor axisColor = workbook.CreateCellsColor();
            axisColor.Color = Color.Gray;
            group.HorizontalAxisColor = axisColor;

            // Guarda el libro de trabajo
            workbook.Save("SparklineWithHorizontalAxis.xlsx");
        }
    }
}
```

### Ver también

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


