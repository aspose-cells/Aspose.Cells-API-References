---
title: "Класс Border"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Border. Инкапсулирует объект, представляющий границу ячейки"
type: docs
url: /ru/net/aspose.cells/border/
---
## Border class

Инкапсулирует объект, представляющий границу ячейки.

```csharp
public class Border
```

## Свойства

| Имя | Описание |
| --- | --- |
| [ArgbColor](../../aspose.cells/border/argbcolor/) { get; set; } | Получает и задаёт цвет в виде 32‑битного значения ARGB. |
| [Color](../../aspose.cells/border/color/) { get; set; } | Получает или задаёт цвет границы. |
| [LineStyle](../../aspose.cells/border/linestyle/) { get; set; } | Получает или задаёт тип границы ячейки. |
| [ThemeColor](../../aspose.cells/border/themecolor/) { get; set; } | Получает и задаёт цвет темы границы. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderDemo
    {
        public static void BorderExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();

            // Добавление нового листа в объект Workbook
            workbook.Worksheets.Add();

            // Получение ссылки на только что добавленный лист путем передачи его индекса листа
            Worksheet worksheet = workbook.Worksheets[0];

            // Доступ к ячейке "A1" листа
            Cell cell = worksheet.Cells["A1"];

            // Добавление некоторого значения в ячейку "A1"
            cell.PutValue("Hello World");

            // Получение стиля ячейки
            Style style = cell.GetStyle();

            // Установка стиля линии верхней границы
            Border topBorder = style.Borders[BorderType.TopBorder];
            topBorder.LineStyle = CellBorderType.Medium;
            topBorder.Color = Color.Red;

            // Установка стиля линии нижней границы
            Border bottomBorder = style.Borders[BorderType.BottomBorder];
            bottomBorder.LineStyle = CellBorderType.Thick;
            bottomBorder.Color = Color.Blue;

            // Установка стиля линии левой границы
            Border leftBorder = style.Borders[BorderType.LeftBorder];
            leftBorder.LineStyle = CellBorderType.Dashed;
            leftBorder.Color = Color.Green;

            // Установка стиля линии правой границы
            Border rightBorder = style.Borders[BorderType.RightBorder];
            rightBorder.LineStyle = CellBorderType.Dotted;
            rightBorder.Color = Color.Purple;

            // Применение стиля к ячейке
            cell.SetStyle(style);

            // Сохранение файла Excel
            workbook.Save("BorderExample.xlsx");
            workbook.Save("BorderExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


