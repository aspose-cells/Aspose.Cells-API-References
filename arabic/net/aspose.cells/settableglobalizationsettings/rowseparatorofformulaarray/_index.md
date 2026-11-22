---
title: "SettableGlobalizationSettings.RowSeparatorOfFormulaArray"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SettableGlobalizationSettings. يحصل على الفاصل للصفوف في بيانات المصفوفة في الصيغة"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/rowseparatorofformulaarray/
---
## SettableGlobalizationSettings.RowSeparatorOfFormulaArray property

يحصل على الفاصل للصفوف في بيانات المصفوفة في الصيغة.

```csharp
public override char RowSeparatorOfFormulaArray { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نسخة من SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // اعرض الفاصل الافتراضي للصفوف لمصفوفات الصيغ
            Console.WriteLine("Default RowSeparatorOfFormulaArray value: " + settings.RowSeparatorOfFormulaArray);

            // حدد فاصل صف جديد لمصفوفات الصيغ
            settings.SetRowSeparatorOfFormulaArray(';');

            // طبق الإعدادات على المصنف
            workbook.Settings.GlobalizationSettings = settings;

            // إنشاء صيغة مصفوفية في ورقة العمل
            worksheet.Cells["A1"].SetArrayFormula("={1,2,3;4,5,6}", 2, 3);
            worksheet.Cells["A2"].SetArrayFormula("=SUM(A1:C2)", 1, 1);

            // حساب الصيغ
            workbook.CalculateFormula();

            // احفظ المصنف
            workbook.Save("PropertyRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


