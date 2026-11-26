---
title: "SparklineGroup.HorizontalAxisDateRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineGroup. Representa el rango que contiene los valores de fecha para los datos del sparkline"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/horizontalaxisdaterange/
---
## SparklineGroup.HorizontalAxisDateRange property

Representa el rango que contiene los valores de fecha para los datos de sparkline.

```csharp
public string HorizontalAxisDateRange { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyHorizontalAxisDateRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de fecha y valor para el sparkline
            sheet.Cells["A1"].PutValue(new DateTime(2023, 1, 1));
            sheet.Cells["B1"].PutValue(new DateTime(2023, 2, 1));
            sheet.Cells["C1"].PutValue(new DateTime(2023, 3, 1));
            sheet.Cells["D1"].PutValue(new DateTime(2023, 4, 1));
            
            sheet.Cells["A2"].PutValue(5);
            sheet.Cells["B2"].PutValue(2);
            sheet.Cells["C2"].PutValue(1);
            sheet.Cells["D2"].PutValue(3);

            // Definir el CellArea donde se colocará el sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 1,
                EndRow = 1
            };

            // Agregar un grupo de sparkline con eje de fecha
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A2:D2", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];
            
            // Establecer el rango de fechas para el eje horizontal
            group.HorizontalAxisDateRange = "A1:D1";
            group.ShowHorizontalAxis = true;

            // Guarda el libro de trabajo
            workbook.Save("SparklineWithDateAxis.xlsx");
        }
    }
}
```

### Ver también

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


