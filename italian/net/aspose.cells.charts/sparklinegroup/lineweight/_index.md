---
title: "SparklineGroup.LineWeight"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SparklineGroup. Ottiene e imposta lo spessore della linea in ogni sparkline lineare nel gruppo di sparkline, nell'unità di punti"
type: docs
url: /it/net/aspose.cells.charts/sparklinegroup/lineweight/
---
## SparklineGroup.LineWeight property

Ottiene e imposta lo spessore della linea in ogni sparkline lineare nel gruppo di sparkline, nell'unità di punti.

```csharp
public double LineWeight { get; set; }
```

### Esempi

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

            // Dati di esempio
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Crea gruppo sparkline
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

            // Imposta la proprietà LineWeight
            group.LineWeight = 2.5; // Thicker line weight for visibility

            workbook.Save("SparklineLineWeightDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


