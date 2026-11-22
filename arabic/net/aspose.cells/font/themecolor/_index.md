---
title: "Font.ThemeColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الخط. تحصل وتعيّن لون السمة"
type: docs
url: /ar/net/aspose.cells/font/themecolor/
---
## Font.ThemeColor property

يحصل على ويضبط لون السمة.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### ملاحظات

إذا لم يكن لون الخط لون سمة، سيتم إرجاع NULL.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyThemeColorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى الخلية A1 وتعيين النص
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Theme Color Demo");

            // احصل على النمط والخط
            Style style = cell.GetStyle();
            Font font = style.Font;

            // إنشاء وتعيين لون السمة
            font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

            // تطبيق النمط على الخلية
            cell.SetStyle(style);

            // احفظ المصنف
            workbook.Save("ThemeColorDemo.xlsx");

            // تحقق من لون السمة
            Font savedFont = worksheet.Cells["A1"].GetStyle().Font;
            Console.WriteLine("ThemeColor Type: " + savedFont.ThemeColor.ColorType);
            Console.WriteLine("ThemeColor Tint: " + savedFont.ThemeColor.Tint);
        }
    }
}
```

### انظر أيضًا

* class [ThemeColor](../../themecolor/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


