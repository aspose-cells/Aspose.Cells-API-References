---
title: "SparklineGroup.PresetStyle"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SparklineGroup. Получает и задает тип предустановленного стиля группы спарклайнов"
type: docs
url: /ru/net/aspose.cells.charts/sparklinegroup/presetstyle/
---
## SparklineGroup.PresetStyle property

Получает и задает тип предустановленного стиля группы спарклайнов.

```csharp
public SparklinePresetStyleType PresetStyle { get; set; }
```

### Примечания

Если это свойство установлено, эти свойства: SeriesColor,NegativePointsColor,HorizontalAxisColor,MarkersColor,FirstPointColor,LastPointColor,HighPointColor,LowPointColor будут переопределены. Поэтому, пожалуйста, сначала установите это свойство, затем установите остальные.

### Примеры

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

            // Пример данных
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(3);
            worksheet.Cells["C1"].PutValue(7);
            worksheet.Cells["D1"].PutValue(2);
            worksheet.Cells["E1"].PutValue(9);

            // Создать группу спарклайнов
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 5;
            ca.EndColumn = 5;
            int index = worksheet.SparklineGroups.Add(SparklineType.Column, "A1:E1", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[index];

            // Применить предустановленный стиль
            group.PresetStyle = SparklinePresetStyleType.Style5;

            workbook.Save("SparklinePresetStyleDemo.xlsx");
        }
    }
}
```

### См. также

* enum [SparklinePresetStyleType](../../sparklinepresetstyletype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


