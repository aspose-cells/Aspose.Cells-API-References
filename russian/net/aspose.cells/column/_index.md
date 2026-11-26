---
title: "Класс Column"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Column. Представляет отдельный столбец в листе."
type: docs
url: /ru/net/aspose.cells/column/
---
## Column class

Представляет отдельный столбец в листе.

```csharp
public class Column
```

## Свойства

| Имя | Описание |
| --- | --- |
| [GroupLevel](../../aspose.cells/column/grouplevel/) { get; set; } | Получает уровень группы столбца. |
| [HasCustomStyle](../../aspose.cells/column/hascustomstyle/) { get; } | Указывает, имеет ли этот столбец пользовательские настройки стиля (отличные от настроек по умолчанию, унаследованных из книги). |
| [Index](../../aspose.cells/column/index/) { get; } | Получает индекс этого столбца. |
| [IsCollapsed](../../aspose.cells/column/iscollapsed/) { get; set; } | является ли столбец свернутым |
| [IsHidden](../../aspose.cells/column/ishidden/) { get; set; } | Указывает, скрыт ли столбец. |
| [Style](../../aspose.cells/column/style/) { get; } | (**Obsolete.**) Получает стиль этого столбца. |
| [Width](../../aspose.cells/column/width/) { get; set; } | Получает и задает ширину столбца в символах. |

## Методы

| Имя | Описание |
| --- | --- |
| [ApplyStyle](../../aspose.cells/column/applystyle/)(Style, StyleFlag) | Применяет форматы ко всему столбцу. |
| [GetStyle](../../aspose.cells/column/getstyle/)() | Получает стиль этого столбца. |
| [SetStyle](../../aspose.cells/column/setstyle/)(Style) | Задает стиль этого столбца. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnDemo
    {
        public static void ColumnExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();

            // Получение ссылки на первый лист
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить новый Style в Workbook
            Style style = workbook.CreateStyle();

            // Установка фонового цвета в синий
            style.BackgroundColor = Color.Blue;

            // Установка цвета переднего плана в красный
            style.ForegroundColor = Color.Red;

            // Установка фонового узора
            style.Pattern = BackgroundType.DiagonalStripe;

            // Новый флаг стиля
            StyleFlag styleFlag = new StyleFlag();

            // Установить все стили
            styleFlag.All = true;

            // Получить первый столбец
            Column column = worksheet.Cells.Columns[0];

            // Применить стиль к первому столбцу
            column.ApplyStyle(style, styleFlag);

            // Настройка дополнительных свойств
            column.Width = 20.0; // Setting the column width
            column.IsHidden = false; // Setting the column visibility
            column.IsCollapsed = false; // Setting the column collapsed state

            // Сохранение файла Excel
            workbook.Save("ColumnExample.xlsx");
            workbook.Save("ColumnExample.pdf");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


