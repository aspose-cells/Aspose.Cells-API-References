---
title: "Перечисление SparklinePresetStyleType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Charts.SparklinePresetStyleType. Представляет предустановленные типы стилей для спарклайна"
type: docs
url: /ru/net/aspose.cells.charts/sparklinepresetstyletype/
---
## SparklinePresetStyleType enumeration

Представляет предустановленные типы стилей спарклайна.

```csharp
public enum SparklinePresetStyleType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Style1 | `0` | Стиль 1 |
| Style2 | `1` | Стиль 2 |
| Style3 | `2` | Стиль 3 |
| Style4 | `3` | Стиль 4 |
| Style5 | `4` | Стиль 5 |
| Style6 | `5` | Стиль 6 |
| Style7 | `6` | Стиль 7 |
| Style8 | `7` | Стиль 8 |
| Style9 | `8` | Стиль 9 |
| Style10 | `9` | Стиль 10 |
| Style11 | `10` | Стиль 11 |
| Style12 | `11` | Стиль 12 |
| Style13 | `12` | Стиль 13 |
| Style14 | `13` | Стиль 14 |
| Style15 | `14` | Стиль 15 |
| Style16 | `15` | Стиль 16 |
| Style17 | `16` | Стиль 17 |
| Style18 | `17` | Стиль 18 |
| Style19 | `18` | Стиль 19 |
| Style20 | `19` | Стиль 20 |
| Style21 | `20` | Стиль 21 |
| Style22 | `21` | Стиль 22 |
| Style23 | `22` | Стиль 23 |
| Style24 | `23` | Стиль 24 |
| Style25 | `24` | Стиль 25 |
| Style26 | `25` | Стиль 26 |
| Style27 | `26` | Стиль 27 |
| Style28 | `27` | Стиль 28 |
| Style29 | `28` | Стиль 29 |
| Style30 | `29` | Стиль 30 |
| Style31 | `30` | Стиль 31 |
| Style32 | `31` | Стиль 32 |
| Style33 | `32` | Стиль 33 |
| Style34 | `33` | Стиль 34 |
| Style35 | `34` | Стиль 35 |
| Style36 | `35` | Стиль 36 |
| Custom | `36` | Нет предустановленного стиля. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklinePresetStyleTypeDemo
    {
        public static void SparklinePresetStyleTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для спарклайнов
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(3);
            worksheet.Cells["D1"].PutValue(4);
            worksheet.Cells["E1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(5);
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["C2"].PutValue(3);
            worksheet.Cells["D2"].PutValue(2);
            worksheet.Cells["E2"].PutValue(1);

            // Определить CellArea для спарклайнов
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 1;
            ca.StartColumn = 5;
            ca.EndColumn = 5;

            // Добавить спарклайны в лист
            int idx = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:E2", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[idx];
            group.Sparklines.Add("A1:E1", 0, 5);
            group.Sparklines.Add("A2:E2", 1, 5);

            // Установить тип предустановленного стиля группы спарклайнов
            group.PresetStyle = SparklinePresetStyleType.Style5;

            // Сохраните книгу
            workbook.Save("SparklinePresetStyleTypeExample.xlsx");

            return;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


