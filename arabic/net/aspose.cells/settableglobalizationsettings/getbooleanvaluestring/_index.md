---
title: "SettableGlobalizationSettings.GetBooleanValueString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. تحصل على قيمة السلسلة المعروضة لقيمة الخلايا المنطقية"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/getbooleanvaluestring/
---
## SettableGlobalizationSettings.GetBooleanValueString method

يحصل على قيمة النص المعروض لقيمة الخلية المنطقية

```csharp
public override string GetBooleanValueString(bool bv)
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

    public class SettableGlobalizationSettingsMethodGetBooleanValueStringWithBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء إعدادات تعميم مخصصة
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // ضبط سلاسل قيم بوليان مخصصة
            settings.SetBooleanValueString(true, "TRUE_CUSTOM");
            settings.SetBooleanValueString(false, "FALSE_CUSTOM");

            // طبق الإعدادات على المصنف
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // استدعِ GetBooleanValueString مع true
                string trueValue = settings.GetBooleanValueString(true);
                Console.WriteLine("Custom true value: " + trueValue);

                // استدعِ GetBooleanValueString مع false
                string falseValue = settings.GetBooleanValueString(false);
                Console.WriteLine("Custom false value: " + falseValue);

                // أظهر التأثير في ورقة العمل
                worksheet.Cells["A1"].PutValue(true);
                worksheet.Cells["A2"].PutValue(false);

                Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2 value: " + worksheet.Cells["A2"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBooleanValueString method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("SettableGlobalizationSettingsMethodGetBooleanValueStringDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


