---
title: "DefaultStyleSettings.FontSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DefaultStyleSettings. تحصل/تعين حجم الخط القياسي الافتراضي لدفتر العمل"
type: docs
url: /ar/net/aspose.cells/defaultstylesettings/fontsize/
---
## DefaultStyleSettings.FontSize property

الحصول/تعيين حجم الخط الافتراضي القياسي لدفتر العمل.

```csharp
public double FontSize { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyFontSizeDemo
    {
        public static void Run()
        {
            HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions();
            
            // تعيين اسم الخط الافتراضي والحجم
            htmlLoadOptions.DefaultStyleSettings.FontName = "Calibri";
            htmlLoadOptions.DefaultStyleSettings.FontSize = 11.0;

            // تحميل ملف HTML بهذه الإعدادات
            Workbook workbook = new Workbook("example.html", htmlLoadOptions);

            // الوصول إلى خلية وعرض حجم الخط الخاص بها
            Cell cell = workbook.Worksheets[0].Cells["A1"];
            Console.WriteLine("Cell A1 Font Size: " + cell.GetStyle().Font.Size);
        }
    }
}
```

### انظر أيضًا

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


