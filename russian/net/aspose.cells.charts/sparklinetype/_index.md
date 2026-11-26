---
title: "Перечисление SparklineType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.SparklineType. Представляет типы спарклайнов"
type: docs
url: /ru/net/aspose.cells.charts/sparklinetype/
---
## SparklineType enumeration

Представляет типы спарклайна.

```csharp
public enum SparklineType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Line | `0` | Линейный спарклайн. |
| Column | `1` | Столбцовый спарклайн. |
| Stacked | `2` | Представляет спарклайн выигрыша/проигрыша. |
| WinLoss | `2` | Представляет спарклайн выигрыша/проигрыша. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class SparklineTypeDemo
    {
        public static void SparklineTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить некоторые данные в лист
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Определите CellArea для спарклайна
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Добавьте группу спарклайнов в лист
            int idx = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[idx];

            // Добавьте спарклайны в группу
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Настройте группу спарклайнов
            CellsColor clr = workbook.CreateCellsColor();
            clr.Color = Color.Orange;
            group.SeriesColor = clr;

            // Установите, чтобы высокие точки были окрашены в зелёный, а низкие — в красный
            group.ShowHighPoint = true;
            group.ShowLowPoint = true;
            group.HighPointColor.Color = Color.Green;
            group.LowPointColor.Color = Color.Red;

            // Установите толщину линии
            group.LineWeight = 1.0;

            // Сохраните книгу
            workbook.Save("SparklineTypeExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


