---
title: "SparklineGroup.VerticalAxisMaxValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SparklineGroup. Получает и задает пользовательское максимальное значение для вертикальной оси"
type: docs
url: /ru/net/aspose.cells.charts/sparklinegroup/verticalaxismaxvalue/
---
## SparklineGroup.VerticalAxisMaxValue property

Получает и задает пользовательское максимальное значение вертикальной оси.

```csharp
public double VerticalAxisMaxValue { get; set; }
```

### Примечания

Если это свойство установлено, [`VerticalAxisMaxValueType`](../verticalaxismaxvaluetype/) будет Custom.

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyVerticalAxisMaxValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Определить расположение спарклайна
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

            // Добавить спарклайн
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Установите максимальное значение вертикальной оси
            group.VerticalAxisMaxValueType = SparklineAxisMinMaxType.Custom;
            group.VerticalAxisMaxValue = 10.0;

            // Сохраните книгу
            workbook.Save("SparklineVerticalAxisMaxValueDemo.xlsx");
        }
    }
}
```

### См. также

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


