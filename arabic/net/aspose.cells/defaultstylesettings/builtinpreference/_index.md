---
title: "DefaultStyleSettings.BuiltInPreference"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DefaultStyleSettings. تشير إلى ما إذا كانت الخاصية لتنسيق الأرقام مفضلة عندما يحدد النمط كلًا من الرقم المدمج والنمط المخصص. القيمة الافتراضية هي false مما يعني أنه بشكل افتراضي سيُستخدم النمط المخصص لتنسيق القيم طالما أنه غير فارغ لنمط واحد."
type: docs
url: /ar/net/aspose.cells/defaultstylesettings/builtinpreference/
---
## DefaultStyleSettings.BuiltInPreference property

يشير إلى ما إذا كانت الخاصية لتنسيق الأرقام مفضلة عندما يحدد النمط كلًا من الرقم المدمج والنمط المخصص. القيمة الافتراضية هي false، وهذا يعني أنه بشكل افتراضي سيُستخدم النمط المخصص لتنسيق القيم طالما أنه غير فارغ لنمط واحد.

```csharp
public bool BuiltInPreference { get; set; }
```

### ملاحظات

عند تحميل دفتر العمل من ملف قالب موجود، قد يتم تعريف كل من الرقم المدمج والنمط المخصص لنمط واحد. تحدد هذه الخاصية ما إذا كنا يجب أن نستخدم الرقم المدمج أو النمط المخصص عند تنسيق القيم باستخدام هذا النمط.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyBuiltInPreferenceDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى إعدادات النمط الافتراضي
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // عرض خاصية BuiltInPreference
            defaultStyleSettings.BuiltInPreference = false;
            defaultStyleSettings.FontName = "Arial";
            defaultStyleSettings.FontSize = 12;

            // تطبيق على ورقة العمل
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text");
            
            // احفظ المصنف
            workbook.Save("BuiltInPreferenceDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


