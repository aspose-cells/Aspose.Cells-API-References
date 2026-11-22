---
title: "Style.ForegroundThemeColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تحصل وتعيّن لون السمة الأمامية"
type: docs
url: /ar/net/aspose.cells/style/foregroundthemecolor/
---
## Style.ForegroundThemeColor property

يحصل على لون سمة المقدمة ويضبطه.

```csharp
public ThemeColor ForegroundThemeColor { get; set; }
```

### ملاحظات

إذا لم يكن لون السمة الأمامية لونًا من السمة، سيتم إرجاع NULL.

### أمثلة

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

### انظر أيضًا

* class [ThemeColor](../../themecolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


