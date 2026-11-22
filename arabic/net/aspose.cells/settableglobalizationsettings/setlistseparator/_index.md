---
title: "SettableGlobalizationSettings.SetListSeparator"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. تحدد الفاصل لمعلمات القائمة في الدالة ...إلخ"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/setlistseparator/
---
## SettableGlobalizationSettings.SetListSeparator method

يضبط الفاصل للقائمة، ومعلمات الدالة، ...إلخ.

```csharp
public void SetListSeparator(char c)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| c | محرف | الفاصل المحدد |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetListSeparatorWithCharDemo
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
                // استدعِ طريقة SetListSeparator مع معامل حرف
                settings.SetListSeparator(';');
                
                // طبق الإعدادات على المصنف
                workbook.Settings.GlobalizationSettings = settings;
                
                // أظهر التأثير بإنشاء صيغة باستخدام فاصل القائمة
                worksheet.Cells["A1"].Formula = "SUM(1;2;3)";
                worksheet.Cells["A2"].Value = "Formula using custom list separator: SUM(1;2;3)";
                
                Console.WriteLine("SetListSeparator method executed successfully with parameter ';'");
                Console.WriteLine("Formula using custom list separator created in cell A1");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetListSeparator method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("SetListSeparatorWithCharDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


