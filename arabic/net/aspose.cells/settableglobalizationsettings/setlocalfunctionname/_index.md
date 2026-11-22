---
title: "SettableGlobalizationSettings.SetLocalFunctionName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. تحدد اسم الدالة المعتمد على اللغة المتطابقة مع اسم الدالة القياسي المعطى"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/setlocalfunctionname/
---
## SettableGlobalizationSettings.SetLocalFunctionName method

يضبط اسم الدالة المعتمد على الإعدادات الإقليمية المتوافق مع اسم الدالة القياسي المعطى.

```csharp
public void SetLocalFunctionName(string standardName, string localName, bool bidirectional)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| standardName | String | اسم الدالة القياسي (إعداد محلي en-US). |
| localName | String | اسم الدالة المعتمد على الإعدادات المحلية |
| bidirectional | Boolean | ما إذا كان سيتم ربط اسم الدالة المحلي باسم الدالة القياسي تلقائيًا. إذا كان true، سيتم ربط الاسم المحلي بالاسم القياسي تلقائيًا بحيث لا يحتاج المستخدم إلى استدعاء [`SetStandardFunctionName`](../setstandardfunctionname/) مرة أخرى لنفس زوج الأسماء القياسية والمحلية |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetLocalFunctionNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أنشئ إعدادات العولمة
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // استدعِ SetLocalFunctionName لربط اسم الدالة القياسي بالاسم المحلي
                settings.SetLocalFunctionName("SUM", "SOMMA", true); // Italian localization for SUM function
                settings.SetLocalFunctionName("AVERAGE", "MEDIA", true); // Italian localization for AVERAGE function

                // طبق الإعدادات على المصنف
                workbook.Settings.GlobalizationSettings = settings;

                // أنشئ صيغًا باستخدام كل من الأسماء القياسية والمحلية
                worksheet.Cells["A1"].Formula = "=SUM(B1:B5)";
                worksheet.Cells["A2"].Formula = "=SOMMA(B1:B5)";
                worksheet.Cells["A3"].Formula = "=AVERAGE(B1:B5)";
                worksheet.Cells["A4"].Formula = "=MEDIA(B1:B5)";

                // حساب الصيغ
                workbook.CalculateFormula();

                Console.WriteLine("SetLocalFunctionName executed successfully with parameters (String, String, Boolean)");
                Console.WriteLine("Standard and localized function names work equivalently in formulas.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLocalFunctionName method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("MethodSetLocalFunctionNameWithStringStringBooleanDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


