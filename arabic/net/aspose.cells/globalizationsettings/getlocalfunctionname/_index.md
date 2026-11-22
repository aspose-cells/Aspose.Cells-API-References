---
title: "GlobalizationSettings.GetLocalFunctionName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GlobalizationSettings. تحصل على اسم الدالة المعتمد على الإعدادات الإقليمية وفقًا لاسم الدالة القياسي المعطى"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/getlocalfunctionname/
---
## GlobalizationSettings.GetLocalFunctionName method

يحصل على اسم الدالة المعتمد على اللغة وفقًا لاسم الدالة المعياري المعطى.

```csharp
public virtual string GetLocalFunctionName(string standardName)
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

    public class GlobalizationSettingsMethodGetLocalFunctionNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين إعدادات العولمة المخصصة
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            // أضف بيانات تجريبية
            worksheet.Cells["B1"].PutValue(5);
            worksheet.Cells["B2"].PutValue(15);

            // إنشاء صيغة باستخدام اسم الدالة المحلي
            Cell cell = worksheet.Cells["B3"];
            cell.Formula = "=LOCALSUM(B1:B2)";

            try
            {
                workbook.CalculateFormula();
                Console.WriteLine($"Calculation result using localized function: {cell.DoubleValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Calculation error: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsFunctionDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetLocalFunctionName(string standardName)
            {
                if (standardName == "SUM")
                {
                    return "LOCALSUM";
                }
                return base.GetLocalFunctionName(standardName);
            }
        }
    }
}
```

### انظر أيضًا

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


