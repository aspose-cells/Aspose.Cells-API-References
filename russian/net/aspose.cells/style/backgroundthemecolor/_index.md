---
title: "Style.BackgroundThemeColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Получает и задает цвет темы фона"
type: docs
url: /ru/net/aspose.cells/style/backgroundthemecolor/
---
## Style.BackgroundThemeColor property

Получает и задает цвет темы фона.

```csharp
public ThemeColor BackgroundThemeColor { get; set; }
```

### Примечания

Если цвет фона не является цветом темы, будет возвращено NULL.

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyBackgroundThemeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создайте стиль и задайте цвет темы фона
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            
            ThemeColor themeColor = new ThemeColor(ThemeColorType.Accent2, 0.5);
            style.BackgroundThemeColor = themeColor;

            // Применить стиль к ячейке
            cells["A1"].SetStyle(style);

            // Проверьте цвет темы фона
            ThemeColor retrievedColor = cells["A1"].GetStyle().BackgroundThemeColor;
            Console.WriteLine("Background Theme Color Type: " + retrievedColor.ColorType);
            Console.WriteLine("Background Theme Color Tint: " + retrievedColor.Tint);
        }
    }
}
```

### См. также

* class [ThemeColor](../../themecolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


