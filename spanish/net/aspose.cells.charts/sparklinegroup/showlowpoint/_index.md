---
title: "SparklineGroup.ShowLowPoint"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineGroup. Indica si se deben resaltar los puntos más bajos de los datos en el grupo de sparklines"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/showlowpoint/
---
## SparklineGroup.ShowLowPoint property

Indica si se debe resaltar los puntos más bajos de datos en el grupo de sparkline.

```csharp
public bool ShowLowPoint { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyShowLowPointDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

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

            group.ShowLowPoint = true;
            group.LowPointColor.Color = Color.Red;

            workbook.Save("SparklineShowLowPointDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


