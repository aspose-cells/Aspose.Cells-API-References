---
title: "Style.ForegroundThemeColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Style. Возвращает и задает цвет темы переднего плана"
type: docs
url: /ru/net/aspose.cells/style/foregroundthemecolor/
---
## Style.ForegroundThemeColor property

Получает и задает цвет переднего плана темы.

```csharp
public ThemeColor ForegroundThemeColor { get; set; }
```

### Примечания

Если цвет переднего плана не является цветом темы, будет возвращено NULL.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyForegroundThemeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            cells["A1"].PutValue("Foreground Theme Color Demo");
            Style style = cells["A1"].GetStyle();

            style.ForegroundThemeColor = new ThemeColor(ThemeColorType.Accent1, -0.25);
            style.Pattern = BackgroundType.Solid;

            cells["A1"].SetStyle(style);
            workbook.Save("ForegroundThemeColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [ThemeColor](../../themecolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


