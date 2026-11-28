---
title: "Style.ForegroundThemeColor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style özelliği. Ön plan tema rengini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/style/foregroundthemecolor/
---
## Style.ForegroundThemeColor property

Ön plan tema rengini alır ve ayarlar.

```csharp
public ThemeColor ForegroundThemeColor { get; set; }
```

### Açıklamalar

Ön plan rengi bir tema rengi değilse, NULL döndürülecektir.

### Örnekler

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

### Ayrıca Bakınız

* class [ThemeColor](../../themecolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


