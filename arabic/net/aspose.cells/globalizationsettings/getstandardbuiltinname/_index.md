---
title: "GlobalizationSettings.GetStandardBuiltInName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GlobalizationSettings. يحصل على النص القياسي للاسم المدمج وفقًا للنص المعتمد على الإعداد المحلي المعطى"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/getstandardbuiltinname/
---
## GlobalizationSettings.GetStandardBuiltInName method

يحصل على النص المعياري للاسم المدمج وفقًا للنص المعتمد على اللغة المعطى.

```csharp
public virtual string GetStandardBuiltInName(string localName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| localName | String | نص معتمد على اللغة للاسم المدمج. تم تحديد اللغة بواسطة المصنف الذي تُستخدم له هذه الإعدادات. |

### قيمة الإرجاع

نص قياسي (لغة en-US).

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف بإعدادات تعميم مخصصة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تهيئة إعدادات التعميم المخصصة وتعيينها إلى المصنف
            var globalizationSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = globalizationSettings;

            // اختبار معلمة لـ GetStandardBuiltInName
            string localFunctionName = "MyLocalSum";
            
            try
            {
                // استدعاء GetStandardBuiltInName مع اسم الدالة المحلي
                string standardName = globalizationSettings.GetStandardBuiltInName(localFunctionName);
                Console.WriteLine($"Local name: '{localFunctionName}' => Standard name: '{standardName}'");

                // إظهار التأثير باستخدام الاسم المحلي في صيغة
                worksheet.Cells["A1"].Value = 5;
                worksheet.Cells["A2"].Value = 7;
                worksheet.Cells["A3"].Formula = $"{localFunctionName}(A1:A2)";

                // احسب الصيغة لإظهار التفسير الصحيح
                workbook.CalculateFormula();
                Console.WriteLine($"Formula result: {worksheet.Cells["A3"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardBuiltInName: {ex.Message}");
            }

            // احفظ المصنف المعدل
            workbook.Save("GlobalizationGetStandardBuiltInNameDemo.xlsx");
        }
    }

    // إعدادات تعميم مخصصة تتجاوز GetStandardBuiltInName
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetStandardBuiltInName(string localName)
        {
            // ربط اسم الدالة المحلية المخصصة بالجمع القياسي SUM
            if (localName.Equals("MyLocalSum", StringComparison.OrdinalIgnoreCase))
            {
                return "SUM";
            }
            return base.GetStandardBuiltInName(localName);
        }
    }
}
```

### انظر أيضًا

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


