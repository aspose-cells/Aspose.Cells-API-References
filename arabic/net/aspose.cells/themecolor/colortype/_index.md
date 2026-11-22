---
title: "ThemeColor.ColorType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThemeColor. تحصل وتضبط نوع السمة"
type: docs
url: /ar/net/aspose.cells/themecolor/colortype/
---
## ThemeColor.ColorType property

يحصل ويضبط نوع السمة.

```csharp
public ThemeColorType ColorType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThemeColorPropertyColorTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء لونين للسمة بأنواع مختلفة
            ThemeColor color1 = new ThemeColor(ThemeColorType.Accent1, 0.5);
            ThemeColor color2 = new ThemeColor(ThemeColorType.Accent2, 0.3);
            
            // عرض خاصية ColorType
            Console.WriteLine("Color1 Type: " + color1.ColorType);
            Console.WriteLine("Color2 Type: " + color2.ColorType);
            
            // تطبيق ألوان السمة على الخلايا
            Style style1 = workbook.CreateStyle();
            style1.ForegroundThemeColor = color1;
            worksheet.Cells["A1"].SetStyle(style1);
            
            Style style2 = workbook.CreateStyle();
            style2.ForegroundThemeColor = color2;
            worksheet.Cells["A2"].SetStyle(style2);
            
            // احفظ المصنف
            workbook.Save("ThemeColorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ThemeColorType](../../themecolortype/)
* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


