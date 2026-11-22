---
title: "SettableGlobalizationSettings.GetLocalFunctionName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. تحصل على اسم الدالة المعتمد على اللغة وفقًا لاسم الدالة القياسي المُعطى"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/getlocalfunctionname/
---
## SettableGlobalizationSettings.GetLocalFunctionName method

يحصل على اسم الدالة المعتمد على اللغة وفقًا لاسم الدالة المعياري المعطى.

```csharp
public override string GetLocalFunctionName(string standardName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| standardName | String | اسم الدالة القياسي (إعداد محلي en-US). |

### قيمة الإرجاع

اسم الدالة المعتمد على الإعداد المحلي. تم تحديد الإعداد المحلي بواسطة Workbook الذي تُستخدم له هذه الإعدادات.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetLocalFunctionNameWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء إعدادات تعميم مخصصة
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // حدد اسم دالة محلية مخصص لـ "SUM"
            settings.SetLocalFunctionName("SUM", "SOMME", true);

            // طبق الإعدادات على المصنف
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // استدعِ GetLocalFunctionName لاسترجاع الاسم المحلي
                string localName = settings.GetLocalFunctionName("SUM");
                
                // اعرض النتيجة
                Console.WriteLine($"Localized function name for 'SUM': {localName}");

                // استخدم الدالة المحلية في خلية
                worksheet.Cells["A1"].Formula = "=SOMME(B1:B5)";
                worksheet.Cells["B1"].PutValue(1);
                worksheet.Cells["B2"].PutValue(2);
                worksheet.Cells["B3"].PutValue(3);
                worksheet.Cells["B4"].PutValue(4);
                worksheet.Cells["B5"].PutValue(5);

                // حساب الصيغ
                workbook.CalculateFormula();

                // اعرض النتيجة
                Console.WriteLine($"Calculation result with localized function: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalFunctionName method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("MethodGetLocalFunctionNameWithStringDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


