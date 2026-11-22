---
title: "SettableGlobalizationSettings.SetBooleanValueString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. يحدد قيمة السلسلة المعروضة للقيمة المنطقية في الخلايا"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/setbooleanvaluestring/
---
## SettableGlobalizationSettings.SetBooleanValueString method

يضبط قيمة سلسلة العرض لقيمة البوليان للخلية

```csharp
public void SetBooleanValueString(bool bv, string name)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| bv | منطقي | قيمة منطقية |
| name | String | قيمة السلسلة للقيمة المنطقية |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetBooleanValueStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء إعدادات تعميم مخصصة
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // ضبط سلاسل قيم بوليان مخصصة
            settings.SetBooleanValueString(true, "Yes");
            settings.SetBooleanValueString(false, "No");
            
            // طبق الإعدادات على المصنف
            workbook.Settings.GlobalizationSettings = settings;
            
            // تعيين قيم منطقية في الخلايا
            worksheet.Cells["A1"].PutValue(true);
            worksheet.Cells["A2"].PutValue(false);
            
            // تعيين نمط العرض لإظهار القيم المنطقية كنص
            Style style = workbook.CreateStyle();
            style.Custom = "BOOLEAN";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A2"].SetStyle(style);
            
            try
            {
                // احفظ المصنف
                workbook.Save("SetBooleanValueStringDemo.xlsx");
                Console.WriteLine("Workbook saved with custom boolean value strings.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


