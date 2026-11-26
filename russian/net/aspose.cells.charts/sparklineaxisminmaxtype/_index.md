---
title: "Перечисление SparklineAxisMinMaxType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.SparklineAxisMinMaxType. Представляет типы минимального и максимального значения для вертикальной оси спарклайна"
type: docs
url: /ru/net/aspose.cells.charts/sparklineaxisminmaxtype/
---
## SparklineAxisMinMaxType enumeration

Представляет типы минимального и максимального значений вертикальной оси спарклайна.

```csharp
public enum SparklineAxisMinMaxType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| AutoIndividual | `0` | Автоматически для каждого спарклайна. |
| Group | `1` | То же для всех спарклайнов в группе. |
| Custom | `2` | Пользовательское значение для спарклайна. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class SparklineAxisMinMaxTypeDemo
    {
        public static void SparklineAxisMinMaxTypeExample()
        {
            // Создайте рабочую книгу и лист
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Определите CellArea
            CellArea cellArea = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Добавьте группу спарклайнов в лист
            int sparklineGroupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup sparklineGroup = worksheet.SparklineGroups[sparklineGroupIndex];
            sparklineGroup.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Установите свойства для группы спарклайнов
            sparklineGroup.VerticalAxisMaxValueType = SparklineAxisMinMaxType.Group;
            sparklineGroup.VerticalAxisMinValueType = SparklineAxisMinMaxType.AutoIndividual;

            // Создайте CellsColor
            CellsColor highPointColor = workbook.CreateCellsColor();
            highPointColor.Color = Color.Green;
            sparklineGroup.HighPointColor = highPointColor;

            CellsColor lowPointColor = workbook.CreateCellsColor();
            lowPointColor.Color = Color.Red;
            sparklineGroup.LowPointColor = lowPointColor;

            // Установить дополнительные свойства
            sparklineGroup.ShowHighPoint = true;
            sparklineGroup.ShowLowPoint = true;
            sparklineGroup.LineWeight = 1.0;

            // Сохраните книгу
            workbook.Save("SparklineAxisMinMaxTypeExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


