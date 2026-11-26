---
title: "Перечисление BorderType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.BorderType. Перечисляет типы линий границы и диагональных линий"
type: docs
url: /ru/net/aspose.cells/bordertype/
---
## BorderType enumeration

Перечисляет типы границ и диагональных линий.

```csharp
[Flags]
public enum BorderType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| LeftBorder | `1` | Представляет левую линию границы. |
| RightBorder | `2` | Представляет существование правой линии границы. |
| TopBorder | `4` | Представляет верхнюю линию границы. |
| BottomBorder | `8` | Представляет нижнюю линию границы. |
| DiagonalDown | `10` | Представляет диагональную линию от верхнего левого к правому нижнему углу. |
| DiagonalUp | `20` | Представляет диагональную линию от нижнего левого к правому верхнему углу. |
| Vertical | `40` | Только для динамического стиля, например условного форматирования, сводных таблиц. |
| Horizontal | `80` | Только для динамического стиля, например условного форматирования, сводных таблиц. |
| SideBorders | `F` | Указывает четыре боковые границы: LeftBorder, RightBorder, TopBorder и BottomBorder. |
| Diagonal | `30` | Специальная комбинация нескольких границ для удобства пользователя в некоторых API. Указывает диагональные границы DiagonalUp и DiagonalDown. |
| DynamicStyleBorders | `C0` | Указывает вертикальные и горизонтальные границы динамического стиля. |
| None | `0` | Границы не указаны. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderTypeDemo
    {
        public static void BorderTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            // Создать диапазон ячеек
            var range = worksheet.Cells.CreateRange("A1:D4");

            // Создать объект стиля
            Style style = workbook.CreateStyle();
            // Установить границы для диапазона
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.DiagonalDown, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.DiagonalUp, CellBorderType.Thin, Color.Blue);

            // Применить стиль к диапазону
            StyleFlag flag = new StyleFlag { Borders = true };
            range.ApplyStyle(style, flag);

            // Сохраните книгу
            workbook.Save("BorderTypeExample.xlsx");
            workbook.Save("BorderTypeExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


