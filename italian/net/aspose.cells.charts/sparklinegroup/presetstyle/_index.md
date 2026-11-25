---
title: "SparklineGroup.PresetStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SparklineGroup. Ottiene e imposta il tipo di stile predefinito del gruppo di sparklines"
type: docs
url: /it/net/aspose.cells.charts/sparklinegroup/presetstyle/
---
## SparklineGroup.PresetStyle property

Ottiene e imposta il tipo di stile predefinito del gruppo di sparkline.

```csharp
public SparklinePresetStyleType PresetStyle { get; set; }
```

### Osservazioni

Se questa proprietà è impostata, queste proprietà: SeriesColor,NegativePointsColor,HorizontalAxisColor,MarkersColor,FirstPointColor,LastPointColor,HighPointColor,LowPointColor saranno coperte. Quindi per favore imposta prima la proprietà, poi imposta le altre.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyPresetStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dati di esempio
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(3);
            worksheet.Cells["C1"].PutValue(7);
            worksheet.Cells["D1"].PutValue(2);
            worksheet.Cells["E1"].PutValue(9);

            // Crea gruppo sparkline
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 5;
            ca.EndColumn = 5;
            int index = worksheet.SparklineGroups.Add(SparklineType.Column, "A1:E1", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[index];

            // Applica stile predefinito
            group.PresetStyle = SparklinePresetStyleType.Style5;

            workbook.Save("SparklinePresetStyleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [SparklinePresetStyleType](../../sparklinepresetstyletype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


