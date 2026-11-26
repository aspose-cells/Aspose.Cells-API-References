---
title: "Font.ThemeColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Font. Получает и задает цвет темы"
type: docs
url: /ru/net/aspose.cells/font/themecolor/
---
## Font.ThemeColor property

Получает и задает цвет темы.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Примечания

Если цвет шрифта не является цветом темы, будет возвращено NULL.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyThemeColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить доступ к ячейке A1 и установить текст
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Theme Color Demo");

            // Получить стиль и шрифт
            Style style = cell.GetStyle();
            Font font = style.Font;

            // Создать и установить цвет темы
            font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

            // Применить стиль к ячейке
            cell.SetStyle(style);

            // Сохраните книгу
            workbook.Save("ThemeColorDemo.xlsx");

            // Проверить цвет темы
            Font savedFont = worksheet.Cells["A1"].GetStyle().Font;
            Console.WriteLine("ThemeColor Type: " + savedFont.ThemeColor.ColorType);
            Console.WriteLine("ThemeColor Tint: " + savedFont.ThemeColor.Tint);
        }
    }
}
```

### См. также

* class [ThemeColor](../../themecolor/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


