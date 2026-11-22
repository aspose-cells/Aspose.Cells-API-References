---
title: "فئة DefaultStyleSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.DefaultStyleSettings فئة. إعدادات القيم الافتراضية لخصائص نمط دفتر العمل"
type: docs
url: /ar/net/aspose.cells/defaultstylesettings/
---
## DefaultStyleSettings class

إعدادات القيم الافتراضية لخصائص نمط المصنف.

```csharp
public class DefaultStyleSettings
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BuiltInPreference](../../aspose.cells/defaultstylesettings/builtinpreference/) { get; set; } | يشير إلى ما إذا كانت الخاصية لتنسيق الأرقام مفضلة عندما يحدد النمط كلًا من الرقم المدمج والنمط المخصص. القيمة الافتراضية هي false، وهذا يعني أنه بشكل افتراضي سيُستخدم النمط المخصص لتنسيق القيم طالما أنه غير فارغ لنمط واحد. |
| [FontName](../../aspose.cells/defaultstylesettings/fontname/) { get; set; } | الحصول/تعيين اسم الخط الافتراضي لدفتر العمل |
| [FontSize](../../aspose.cells/defaultstylesettings/fontsize/) { get; set; } | الحصول/تعيين حجم الخط الافتراضي القياسي لدفتر العمل. |
| [HorizontalAlignment](../../aspose.cells/defaultstylesettings/horizontalalignment/) { get; set; } | الحصول/تعيين القيمة الافتراضية للمحاذاة الأفقية |
| [VerticalAlignment](../../aspose.cells/defaultstylesettings/verticalalignment/) { get; set; } | الحصول/تعيين القيمة الافتراضية للمحاذاة العمودية |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DefaultStyleSettingsDemo
    {
        public static void DefaultStyleSettingsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى إعدادات النمط الافتراضية لدفتر العمل
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // ضبط الخصائص
            defaultStyleSettings.BuiltInPreference = false;
            defaultStyleSettings.FontName = "Arial";
            defaultStyleSettings.FontSize = 12.0;
            defaultStyleSettings.HorizontalAlignment = TextAlignmentType.Center;
            defaultStyleSettings.VerticalAlignment = TextAlignmentType.Center;

            // تطبيق إعدادات النمط الافتراضية على ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells.ApplyStyle(workbook.CreateStyle(), new StyleFlag() { All = true });

            // احفظ المصنف
            workbook.Save("DefaultStyleSettingsExample.xlsx");
            workbook.Save("DefaultStyleSettingsExample.pdf");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


