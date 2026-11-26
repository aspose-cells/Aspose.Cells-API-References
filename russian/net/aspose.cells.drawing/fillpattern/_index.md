---
title: "Перечисление FillPattern"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.Drawing.FillPattern. Перечисляет типы шаблонов заливки фигур"
type: docs
url: /ru/net/aspose.cells.drawing/fillpattern/
---
## FillPattern enumeration

Перечисляет типы шаблонов заливки фигуры.

```csharp
public enum FillPattern
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Представляет отсутствие фона. |
| Solid | `1` | Представляет сплошной узор. |
| Gray5 | `2` | Представляет шаблон 5% серого. |
| Gray10 | `3` | Представляет шаблон 10% серого. |
| Gray20 | `4` | Представляет шаблон 20% серого. |
| Gray30 | `5` | Представляет шаблон 30% серого. |
| Gray40 | `6` | Представляет шаблон 40% серого. |
| Gray50 | `7` | Представляет шаблон серого 50%. |
| Gray60 | `8` | Представляет шаблон 60% серого. |
| Gray70 | `9` | Представляет шаблон 70% серого. |
| Gray75 | `10` | Представляет шаблон серого 75%. |
| Gray80 | `11` | Представляет шаблон 80% серого. |
| Gray90 | `12` | Представляет шаблон 90% серого. |
| Gray25 | `13` | Представляет шаблон серого 25%. |
| LightDownwardDiagonal | `14` | Представляет светлый нисходящий диагональный шаблон. |
| LightUpwardDiagonal | `15` | Представляет светлый восходящий диагональный шаблон. |
| DarkDownwardDiagonal | `16` | Представляет тёмный нисходящий диагональный шаблон. |
| DarkUpwardDiagonal | `17` | Представляет тёмный восходящий диагональный шаблон. |
| WideDownwardDiagonal | `18` | Представляет широкий нисходящий диагональный шаблон. |
| WideUpwardDiagonal | `19` | Представляет широкий восходящий диагональный шаблон. |
| LightVertical | `20` | Представляет светлый вертикальный шаблон. |
| LightHorizontal | `21` | Представляет светлый горизонтальный шаблон. |
| NarrowVertical | `22` | Представляет узкий вертикальный шаблон. |
| NarrowHorizontal | `23` | Представляет узкий горизонтальный шаблон. |
| DarkVertical | `24` | Представляет тёмный вертикальный шаблон. |
| DarkHorizontal | `25` | Представляет тёмный горизонтальный шаблон. |
| DashedDownwardDiagonal | `26` | Представляет пунктирный нисходящий диагональный шаблон. |
| DashedUpwardDiagonal | `27` | Представляет пунктирный восходящий диагональный шаблон. |
| DashedVertical | `28` | Представляет пунктирный вертикальный шаблон. |
| DashedHorizontal | `29` | Представляет пунктирный горизонтальный шаблон. |
| SmallConfetti | `30` | Представляет малый шаблон конфетти. |
| LargeConfetti | `31` | Представляет большой шаблон конфетти. |
| ZigZag | `32` | Представляет зигзагообразный шаблон. |
| Wave | `33` | Представляет волнообразный шаблон. |
| DiagonalBrick | `34` | Представляет диагональный кирпичный шаблон. |
| HorizontalBrick | `35` | Представляет горизонтальный кирпичный шаблон. |
| Weave | `36` | Представляет шаблон плетения. |
| Plaid | `37` | Представляет узор в клетку. |
| Divot | `38` | Представляет узор с вмятинами. |
| DottedGrid | `39` | Представляет узор точечной сетки. |
| DottedDiamond | `40` | Представляет узор точечного ромба. |
| Shingle | `41` | Представляет узор черепицы. |
| Trellis | `42` | Представляет узор решетки. |
| Sphere | `43` | Представляет узор сферы. |
| SmallGrid | `44` | Представляет узор маленькой сетки. |
| LargeGrid | `45` | Представляет узор большой сетки. |
| SmallCheckerBoard | `46` | Представляет узор маленькой шахматной доски. |
| LargeCheckerBoard | `47` | Представляет узор большой шахматной доски. |
| OutlinedDiamond | `48` | Представляет узор контурного ромба. |
| SolidDiamond | `49` | Представляет узор сплошного ромба. |
| Unknown | `50` | Представляет неизвестный узор. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassFillPatternDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить примерные данные для диаграммы
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Добавьте диаграмму
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Установить диапазон данных диаграммы
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Установить шаблон заливки для первой серии
            Series series = chart.NSeries[0];
            series.Area.FillFormat.Pattern = FillPattern.Plaid;

            // Сохраните книгу
            workbook.Save("FillPatternDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


