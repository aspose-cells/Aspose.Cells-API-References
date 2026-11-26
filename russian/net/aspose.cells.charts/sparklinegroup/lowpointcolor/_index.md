---
title: "SparklineGroup.LowPointColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SparklineGroup. Получает и задает цвет самых низких точек данных в группе спарклайнов"
type: docs
url: /ru/net/aspose.cells.charts/sparklinegroup/lowpointcolor/
---
## SparklineGroup.LowPointColor property

Получает и задает цвет самых низких точек данных в группе спарклайнов.

```csharp
public CellsColor LowPointColor { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyLowPointColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Пример данных
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Создать группу спарклайнов
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Добавить группу спарклайнов, используя правильный API
            int idx = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[idx];
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Настроить внешний вид спарклайна
            group.ShowLowPoint = true;
            group.LowPointColor.Color = Color.Red;

            workbook.Save("SparklineLowPointColorDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


