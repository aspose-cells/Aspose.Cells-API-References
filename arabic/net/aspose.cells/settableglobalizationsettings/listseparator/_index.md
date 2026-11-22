---
title: "SettableGlobalizationSettings.ListSeparator"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SettableGlobalizationSettings. يحصل على الفاصل لمعلمات القائمة في الدالة ...إلخ"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/listseparator/
---
## SettableGlobalizationSettings.ListSeparator property

يحصل على الفاصل للقائمة، معلمات الدالة، ...إلخ.

```csharp
public override char ListSeparator { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyListSeparatorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نسخة من SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // اعرض قيمة ListSeparator الحالية (الافتراضي هو الفاصلة في معظم اللغات)
            Console.WriteLine("Current ListSeparator value: " + settings.ListSeparator);
            
            // حدد قيمة ListSeparator جديدة (مثال: الفاصلة المنقوطة)
            settings.SetListSeparator(';');
            
            // طبق الإعدادات على المصنف
            workbook.Settings.GlobalizationSettings = settings;
            
            // أظهر تأثير ListSeparator في تحليل الصيغ
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["A2"].PutValue("Data");
            
            // أنشئ صيغة تستخدم فاصل القائمة
            worksheet.Cells["A3"].Formula = "=CONCATENATE(A1,A2)";
            
            // ستستخدم الصيغة فاصل القائمة المخصص عند التحليل
            Console.WriteLine("Formula with custom separator: " + worksheet.Cells["A3"].Formula);
            
            // احفظ المصنف
            workbook.Save("PropertyListSeparatorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


