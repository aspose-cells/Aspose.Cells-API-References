---
title: "GlobalizationSettings.ListSeparator"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GlobalizationSettings. يحصل على الفاصل لمعلمات القائمة في الدالة ...إلخ"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/listseparator/
---
## GlobalizationSettings.ListSeparator property

يحصل على الفاصل للقائمة، معلمات الدالة، ...إلخ.

```csharp
public virtual char ListSeparator { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyListSeparatorDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد بإعدادات عولمة مخصصة
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            Worksheet worksheet = workbook.Worksheets[0];
            
            // عرض قيمة ListSeparator الحالية من إعداداتنا المخصصة
            Console.WriteLine("Current ListSeparator value: " + workbook.Settings.GlobalizationSettings.ListSeparator);

            // إنشاء صيغة باستخدام فاصل القائمة المخصص
            worksheet.Cells["A1"].Formula = "=CONCATENATE(\"Hello\"; \" World\")";
            worksheet.Cells["A2"].Formula = "=SUM(1;2;3)";

            // احسب الصيغ باستخدام الفاصل المخصص
            workbook.CalculateFormula();

            // إظهار نتائج الحساب
            Console.WriteLine("Concatenation result: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Sum result: " + worksheet.Cells["A2"].Value);

            // حفظ مع الصيغ باستخدام فاصل القائمة المخصص
            workbook.Save("ListSeparatorDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override char ListSeparator => ';';
        }
    }
}
```

### انظر أيضًا

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


