---
title: "SettableGlobalizationSettings.SetRowSeparatorOfFormulaArray"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. يحدد الفاصل للصفوف في بيانات المصفوفة في الصيغة"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/setrowseparatorofformulaarray/
---
## SettableGlobalizationSettings.SetRowSeparatorOfFormulaArray method

يضبط الفاصل للصفوف في بيانات المصفوفة في الصيغة.

```csharp
public void SetRowSeparatorOfFormulaArray(char c)
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

    public class SettableGlobalizationSettingsMethodSetRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء إعدادات تعميم مخصصة
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // تعيين فاصل الصفوف لمصفوفات الصيغ إلى '|'
            char rowSeparator = '|';
            settings.SetRowSeparatorOfFormulaArray(rowSeparator);

            // طبق الإعدادات على المصنف
            workbook.Settings.GlobalizationSettings = settings;

            // إنشاء صيغة مصفوفية في ورقة العمل
            worksheet.Cells["A1"].SetArrayFormula("={1,2,3;4,5,6}", 2, 3);
            
            try
            {
                // حساب الصيغة لتطبيق الإعدادات
                workbook.CalculateFormula();

                // عرض الصيغة مع الفاصل الصفّي الجديد
                Console.WriteLine("Array formula with custom row separator: " + worksheet.Cells["A1"].Formula);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetRowSeparatorOfFormulaArray method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("MethodSetRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


