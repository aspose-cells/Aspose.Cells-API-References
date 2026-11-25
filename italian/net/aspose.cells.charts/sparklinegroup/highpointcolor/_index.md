---
title: "SparklineGroup.HighPointColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SparklineGroup. Ottiene e imposta il colore dei punti più alti dei dati nel gruppo di sparkline"
type: docs
url: /it/net/aspose.cells.charts/sparklinegroup/highpointcolor/
---
## SparklineGroup.HighPointColor property

Ottiene e imposta il colore dei punti più alti dei dati nel gruppo di sparkline.

```csharp
public CellsColor HighPointColor { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyHighPointColorDemo
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

            group.ShowHighPoint = true;
            group.HighPointColor.Color = Color.Green;

            workbook.Save("SparklineHighPointColorDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


