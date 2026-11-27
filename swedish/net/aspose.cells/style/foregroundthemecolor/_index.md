---
title: "Style.ForegroundThemeColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Hämtar och anger förgrundens temafärg"
type: docs
url: /sv/net/aspose.cells/style/foregroundthemecolor/
---
## Style.ForegroundThemeColor property

Hämtar och anger förgrundens temafärg.

```csharp
public ThemeColor ForegroundThemeColor { get; set; }
```

### Anmärkningar

Om förgrundsfärgen inte är en temafärg returneras NULL.

### Exempel

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

### Se även

* class [ThemeColor](../../themecolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


