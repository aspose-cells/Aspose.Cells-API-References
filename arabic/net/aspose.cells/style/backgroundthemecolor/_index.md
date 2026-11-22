---
title: "Style.BackgroundThemeColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Style property. يحصل على ويضبط لون السمة الخلفية"
type: docs
url: /ar/net/aspose.cells/style/backgroundthemecolor/
---
## Style.BackgroundThemeColor property

يحصل على لون سمة الخلفية ويضبطه.

```csharp
public ThemeColor BackgroundThemeColor { get; set; }
```

### ملاحظات

إذا لم يكن لون الخلفية لون سمة، سيتم إرجاع NULL.

### أمثلة

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

            // إنشاء نمط وتعيين لون سمة الخلفية
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            
            ThemeColor themeColor = new ThemeColor(ThemeColorType.Accent2, 0.5);
            style.BackgroundThemeColor = themeColor;

            // تطبيق النمط على خلية
            cells["A1"].SetStyle(style);

            // تحقق من لون سمة الخلفية
            ThemeColor retrievedColor = cells["A1"].GetStyle().BackgroundThemeColor;
            Console.WriteLine("Background Theme Color Type: " + retrievedColor.ColorType);
            Console.WriteLine("Background Theme Color Tint: " + retrievedColor.Tint);
        }
    }
}
```

### انظر أيضًا

* class [ThemeColor](../../themecolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


