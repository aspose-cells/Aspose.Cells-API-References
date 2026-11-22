---
title: "SettableGlobalizationSettings.SetStandardFunctionName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. تعيين اسم الدالة المعتمد على الإعدادات المحلية وفقًا لاسم الدالة القياسي المعطى"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/setstandardfunctionname/
---
## SettableGlobalizationSettings.SetStandardFunctionName method

يضبط اسم الدالة المعتمد على الإعدادات الإقليمية وفقًا لاسم الدالة القياسي المعطى.

```csharp
public void SetStandardFunctionName(string localName, string standardName, bool bidirectional)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| localName | String | اسم الدالة المعتمد على الإعدادات المحلية |
| standardName | String | اسم الدالة القياسي (إعداد محلي en-US). |
| bidirectional | Boolean | ما إذا كان سيتم ربط اسم الدالة القياسي باسم الدالة المحلي تلقائيًا. إذا كان صحيحًا، سيتم ربط الاسم القياسي بالاسم المحلي تلقائيًا بحيث لا يحتاج المستخدم إلى استدعاء [`SetLocalFunctionName`](../setlocalfunctionname/) مرة أخرى لنفس زوج الأسماء القياسية والمحلية |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardFunctionNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء إعدادات تعميم مخصصة
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // استدعِ SetStandardFunctionName لربط اسم دالة محلية بالاسم القياسي
                settings.SetStandardFunctionName("LOCAL_SUM", "SUM", true);

                // تطبيق الإعدادات على المصنف
                workbook.Settings.GlobalizationSettings = settings;

                // إنشاء صيغة باستخدام اسم الدالة المحلي
                worksheet.Cells["A1"].Formula = "=LOCAL_SUM(B1:B3)";
                worksheet.Cells["B1"].Value = 10;
                worksheet.Cells["B2"].Value = 20;
                worksheet.Cells["B3"].Value = 30;

                // احسب الصيغة
                workbook.CalculateFormula();

                Console.WriteLine("Formula with local function name 'LOCAL_SUM' calculated successfully.");
                Console.WriteLine($"Result: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardFunctionName method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("SetStandardFunctionNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


