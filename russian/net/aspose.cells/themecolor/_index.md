---
title: "Класс ThemeColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ThemeColor. Представляет цвет темы"
type: docs
url: /ru/net/aspose.cells/themecolor/
---
## ThemeColor class

Представляет цвет темы.

```csharp
public class ThemeColor
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ThemeColor](themecolor/)(ThemeColorType, double) |  |

## Свойства

| Имя | Описание |
| --- | --- |
| [ColorType](../../aspose.cells/themecolor/colortype/) { get; set; } | Получает и задает тип темы. |
| [Tint](../../aspose.cells/themecolor/tint/) { get; set; } | Получает и задает значение оттенка. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThemeColorDemo
    {
        public static void ThemeColorExample()
        {
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Добавление значения в ячейку A1
            cells["A1"].PutValue("Hello World");

            // Получение стиля ячейки A1
            Style style = cells["A1"].GetStyle();

            // Установить тип цвета ThemeColorType.Text2 с осветлением на 40% в качестве цвета шрифта.
            style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text2, 0.4);
            style.Pattern = BackgroundType.Solid;

            // Установить тип цвета ThemeColorType.Background2 с затемнением на 75% в качестве цвета переднего плана.
            style.ForegroundThemeColor = new ThemeColor(ThemeColorType.Background2, -0.75);

            // Применение стиля к ячейке A1
            cells["A1"].SetStyle(style);

            // Сохранение файла Excel
            workbook.Save("ThemeColorExample.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


