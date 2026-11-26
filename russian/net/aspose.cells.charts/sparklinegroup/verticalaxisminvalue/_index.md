---
title: "SparklineGroup.VerticalAxisMinValue"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SparklineGroup. Получает и задает пользовательское минимальное значение вертикальной оси"
type: docs
url: /ru/net/aspose.cells.charts/sparklinegroup/verticalaxisminvalue/
---
## SparklineGroup.VerticalAxisMinValue property

Получает и задает пользовательское минимальное значение вертикальной оси.

```csharp
public double VerticalAxisMinValue { get; set; }
```

### Примечания

Если это свойство установлено, [`VerticalAxisMinValueType`](../verticalaxisminvaluetype/) будет Custom.

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyVerticalAxisMinValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["A2"].PutValue(2);
            sheet.Cells["A3"].PutValue(1);
            sheet.Cells["A4"].PutValue(3);

            // Создать группу спарклайнов
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 3;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:A4", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Установить минимальное значение вертикальной оси
            group.VerticalAxisMinValueType = SparklineAxisMinMaxType.Custom;
            group.VerticalAxisMinValue = 0.0;

            // Сохраните книгу
            workbook.Save("SparklineVerticalAxisMinValueDemo.xlsx");
        }
    }
}
```

### См. также

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


