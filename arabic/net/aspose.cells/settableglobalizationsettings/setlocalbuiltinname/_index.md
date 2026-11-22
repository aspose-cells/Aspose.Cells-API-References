---
title: "SettableGlobalizationSettings.SetLocalBuiltInName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. تعيين النص المعتمد على الإعدادات المحلية لاسم المدمج باستخدام نص الاسم القياسي المعطى"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/setlocalbuiltinname/
---
## SettableGlobalizationSettings.SetLocalBuiltInName method

يضبط النص المعتمد على الإعدادات الإقليمية للاسم المدمج بالنص القياسي المعطى.

```csharp
public void SetLocalBuiltInName(string standardName, string localName, bool bidirectional)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| standardName | String | نص الاسم القياسي (en-US locale) للاسم المدمج. |
| localName | String | نص الاسم المعتمد على الإعدادات المحلية |
| bidirectional | Boolean | ما إذا كان سيتم ربط نص الاسم المحلي بنص الاسم القياسي تلقائيًا. إذا كان صحيحًا، سيتم ربط نص الاسم المحلي بنص الاسم القياسي تلقائيًا بحيث لا يحتاج المستخدم إلى استدعاء [`SetStandardBuiltInName`](../setstandardbuiltinname/) مرة أخرى لنفس زوج الأسماء القياسية والمحلية |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetLocalBuiltInNameWithStringStringBooleanDemo
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
                // استدعِ SetLocalBuiltInName لربط اسم مدمج قياسي باسم محلي
                settings.SetLocalBuiltInName("SUM", "LOCAL_SUM", true);

                // طبق الإعدادات على المصنف
                workbook.Settings.GlobalizationSettings = settings;

                // إنشاء صيغة باستخدام الاسم المدمج القياسي
                worksheet.Cells["A1"].Formula = "=SUM(B1:B3)";
                worksheet.Cells["B1"].Value = 5;
                worksheet.Cells["B2"].Value = 10;
                worksheet.Cells["B3"].Value = 15;

                // احسب الصيغة
                workbook.CalculateFormula();

                Console.WriteLine("Formula with standard built-in name 'SUM' calculated successfully.");
                Console.WriteLine($"Result: {worksheet.Cells["A1"].Value}");

                // تحقق من ربط الاسم المحلي
                string localName = settings.GetLocalBuiltInName("SUM");
                Console.WriteLine($"Local name for 'SUM': {localName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLocalBuiltInName method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("SetLocalBuiltInNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


