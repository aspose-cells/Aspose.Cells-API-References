---
title: "GlobalizationSettings.GetStandardFunctionName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GlobalizationSettings. يحصل على اسم الدالة القياسي وفقًا لاسم الدالة المعتمد على الإعداد الإقليمي المعطى"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/getstandardfunctionname/
---
## GlobalizationSettings.GetStandardFunctionName method

يحصل على اسم الدالة المعياري وفقًا لاسم الدالة المعتمد على اللغة المعطى.

```csharp
public virtual string GetStandardFunctionName(string localName)
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

    public class GlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تحضير بيانات عينة
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(15);
            
            // إنشاء إعدادات عولمة مخصصة وتعيينها إلى المصنف
            var customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // عرض GetStandardFunctionName باستخدام اسم الدالة SUM الألماني
                string localName = "SUMME";
                string standardName = customSettings.GetStandardFunctionName(localName);
                
                Console.WriteLine($"Local function name: {localName}");
                Console.WriteLine($"Standard function name: {standardName}");

                // تطبيق اسم الدالة المحلي في الصيغة
                worksheet.Cells["A3"].Formula = "=SUMME(A1:A2)";
                workbook.CalculateFormula();
                
                Console.WriteLine($"Formula result: {worksheet.Cells["A3"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardFunctionName method: {ex.Message}");
            }

            workbook.Save("MethodGetStandardFunctionNameDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetStandardFunctionName(string localName)
            {
                // تحويل اسم الدالة الألماني إلى الإنجليزية القياسية
                if (localName.Equals("SUMME", StringComparison.OrdinalIgnoreCase))
                {
                    return "SUM";
                }
                return base.GetStandardFunctionName(localName);
            }
        }
    }
}
```

### انظر أيضًا

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


