---
title: "SparklineGroup.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineGroup. Indica el tipo de sparkline del grupo de sparklines"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/type/
---
## SparklineGroup.Type property

Indica el tipo de sparkline del grupo de sparkline.

```csharp
public SparklineType Type { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyTypeDemo
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

            // Crear grupo de sparkline con tipo Column
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Column, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Cambiar el tipo de sparkline a Line
            group.Type = SparklineType.Line;

            // Agregar sparkline al grupo
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Guarda el libro de trabajo
            workbook.Save("SparklineTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [SparklineType](../../sparklinetype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


