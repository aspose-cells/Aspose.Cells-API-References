---
title: "SettableGlobalizationSettings.GetStandardBuiltInName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. تحصل على النص القياسي للاسم المدمج وفقًا للنص المعتمد على اللغة المُعطى"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/getstandardbuiltinname/
---
## SettableGlobalizationSettings.GetStandardBuiltInName method

يحصل على النص المعياري للاسم المدمج وفقًا للنص المعتمد على اللغة المعطى.

```csharp
public override string GetStandardBuiltInName(string localName)
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

    public class SettableGlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نسخة من SettableGlobalizationSettings
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            // حدد اسمًا مدمجًا محليًا للتوضيح
            globalizationSettings.SetLocalBuiltInName("SUM", "LocalSumName", true);

            try
            {
                // استدعِ طريقة GetStandardBuiltInName باسم محلي
                string standardName = globalizationSettings.GetStandardBuiltInName("LocalSumName");
                
                // اعرض النتيجة
                Console.WriteLine($"Standard name for 'LocalSumName' is: {standardName}");

                // طبق النتيجة على خلية
                worksheet.Cells["A1"].Formula = "=" + standardName + "(1,2,3)";
                workbook.CalculateFormula();

                // اعرض النتيجة المحسوبة
                Console.WriteLine($"Result of formula in A1: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardBuiltInName method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("SettableGlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


