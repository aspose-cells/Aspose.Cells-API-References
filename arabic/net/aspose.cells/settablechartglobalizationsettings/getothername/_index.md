---
title: "SettableChartGlobalizationSettings.GetOtherName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableChartGlobalizationSettings. تحصل على اسم تسميات Other للمخطط"
type: docs
url: /ar/net/aspose.cells/settablechartglobalizationsettings/getothername/
---
## SettableChartGlobalizationSettings.GetOtherName method

يحصل على اسم تسميات "Other" للمخطط.

```csharp
public override string GetOtherName()
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetOtherNameDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات قليلة (اختياري، فقط للحصول على دفتر عمل كامل)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(250);

            try
            {
                // إنشاء كائن إعدادات العولمة
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // تعيين اسم مخصص لتسمية "Other"
                settings.SetOtherName("Custom Other Label");

                // استرجاع الاسم باستخدام GetOtherName
                string otherName = settings.GetOtherName();

                Console.WriteLine("Other Name retrieved: " + otherName);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetOtherName: {ex.Message}");
            }

            // حفظ دفتر العمل (الإعدادات غير مرتبطة مباشرة بالمخطط في هذا العرض)
            workbook.Save("GetOtherNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


