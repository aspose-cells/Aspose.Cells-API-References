---
title: "SparklineGroup.VerticalAxisMinValueType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SparklineGroup. Представляет тип минимального значения вертикальной оси"
type: docs
url: /ru/net/aspose.cells.charts/sparklinegroup/verticalaxisminvaluetype/
---
## SparklineGroup.VerticalAxisMinValueType property

Представляет тип минимального значения вертикальной оси.

```csharp
public SparklineAxisMinMaxType VerticalAxisMinValueType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyVerticalAxisMinValueTypeDemo
    {
        public static void Run()
        {
            // Создайте рабочую книгу и лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Определить расположение спарклайна
            CellArea cellArea = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Добавить группу спарклайнов
            int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup group = worksheet.SparklineGroups[groupIndex];
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Установить тип минимального значения вертикальной оси
            group.VerticalAxisMinValueType = SparklineAxisMinMaxType.AutoIndividual;

            // Сохраните книгу
            workbook.Save("SparklineVerticalAxisMinValueTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [SparklineAxisMinMaxType](../../sparklineaxisminmaxtype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


