---
title: "SparklineGroup.PlotEmptyCellsType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SparklineGroup. Указывает, как отображать пустые ячейки"
type: docs
url: /ru/net/aspose.cells.charts/sparklinegroup/plotemptycellstype/
---
## SparklineGroup.PlotEmptyCellsType property

Указывает, как отображать пустые ячейки.

```csharp
public PlotEmptyCellsType PlotEmptyCellsType { get; set; }
```

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyPlotEmptyCellsTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте данные с некоторыми пустыми ячейками
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(null); // Empty cell
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Определите CellArea для спарклайна
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Добавить группу спарклайнов
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Установите, как должны отображаться пустые ячейки
            group.PlotEmptyCellsType = PlotEmptyCellsType.Zero;

            // Добавить спарклайн в группу
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Сохраните книгу
            workbook.Save("SparklineEmptyCellsDemo.xlsx");
        }
    }
}
```

### См. также

* enum [PlotEmptyCellsType](../../plotemptycellstype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


