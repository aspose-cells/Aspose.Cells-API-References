---
title: "SettableGlobalizationSettings.GetStandardFunctionName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. تحصل على اسم الدالة القياسي وفقًا لاسم الدالة المعتمد على الإعداد المحلي المعطى"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/getstandardfunctionname/
---
## SettableGlobalizationSettings.GetStandardFunctionName method

يحصل على اسم الدالة المعياري وفقًا لاسم الدالة المعتمد على اللغة المعطى.

```csharp
public override string GetStandardFunctionName(string localName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| localName | String | اسم الدالة المعتمد على الإعداد المحلي. تم تحديد الإعداد المحلي بواسطة Workbook الذي تُستخدم له هذه الإعدادات. |

### قيمة الإرجاع

اسم الدالة القياسي (إعداد محلي en-US).

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء إعدادات تعميم مخصصة
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // حدد تعيين اسم الدالة المحلية
            settings.SetStandardFunctionName("LocalSum", "SUM", true);

            // طبق الإعدادات على المصنف
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // استدعِ GetStandardFunctionName باسم دالة محلية
                string standardName = settings.GetStandardFunctionName("LocalSum");
                
                // اعرض النتيجة
                Console.WriteLine($"Standard function name for 'LocalSum' is: {standardName}");

                // استخدم الدالة القياسية في صيغة خلية
                worksheet.Cells["A1"].Formula = $"={standardName}(1,2,3)";
                worksheet.Cells["A2"].Value = 1;
                worksheet.Cells["A3"].Value = 2;
                worksheet.Cells["A4"].Value = 3;

                // احسب الصيغة
                workbook.CalculateFormula();

                // اعرض النتيجة
                Console.WriteLine($"Formula result in A1: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardFunctionName method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("SettableGlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


