---
title: "GlobalizationSettings.GetBooleanValueString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GlobalizationSettings. تحصل على قيمة السلسلة المعروضة لقيمة الخلايا المنطقية"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/getbooleanvaluestring/
---
## GlobalizationSettings.GetBooleanValueString method

يحصل على قيمة النص المعروض لقيمة الخلية المنطقية

```csharp
public virtual string GetBooleanValueString(bool bv)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| bv | منطقي | قيمة منطقية |

### قيمة الإرجاع

بشكل افتراضي تُعيد "TRUE" للقيمة true و"FALSE" للقيمة false.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetBooleanValueStringWithBooleanDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد بإعدادات عولمة مخصصة
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomBooleanGlobalizationSettings();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // عرض GetBooleanValueString مع كلا القيمتين المنطقيتين
                var globalizationSettings = workbook.Settings.GlobalizationSettings;
                string trueResult = globalizationSettings.GetBooleanValueString(true);
                string falseResult = globalizationSettings.GetBooleanValueString(false);

                Console.WriteLine($"GetBooleanValueString(true) returns: {trueResult}");
                Console.WriteLine($"GetBooleanValueString(false) returns: {falseResult}");

                // تطبيق القيم المنطقية على الخلايا لإظهار تأثير الجدول الإلكتروني
                worksheet.Cells["A1"].PutValue(true);
                worksheet.Cells["A2"].PutValue(false);

                workbook.Save("GlobalizationBooleanDemo.xlsx");
                Console.WriteLine("Workbook saved with custom boolean representations.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBooleanValueString: {ex.Message}");
            }
        }
    }

    // إعدادات عولمة مخصصة تتجاوز تمثيل السلسلة المنطقية
    public class CustomBooleanGlobalizationSettings : GlobalizationSettings
    {
        public override string GetBooleanValueString(bool bv)
        {
            return bv ? "Enabled" : "Disabled";
        }
    }
}
```

### انظر أيضًا

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


