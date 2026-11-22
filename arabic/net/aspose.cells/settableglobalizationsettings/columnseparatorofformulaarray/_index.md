---
title: "SettableGlobalizationSettings.ColumnSeparatorOfFormulaArray"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SettableGlobalizationSettings. تحصل على الفاصل للعناصر في صفوف البيانات بالمصفوفات في الصيغة"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/columnseparatorofformulaarray/
---
## SettableGlobalizationSettings.ColumnSeparatorOfFormulaArray property

يحصل على الفاصل للعناصر في بيانات صف المصفوفة في الصيغة.

```csharp
public override char ColumnSeparatorOfFormulaArray { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsPropertyColumnSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نسخة من SettableGlobalizationSettings
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            // عرض القيمة الحالية لـ ColumnSeparatorOfFormulaArray
            Console.WriteLine("Current ColumnSeparatorOfFormulaArray value: " + settings.ColumnSeparatorOfFormulaArray);

            // تعيين قيمة جديدة لـ ColumnSeparatorOfFormulaArray
            settings.SetColumnSeparatorOfFormulaArray(';');

            // تطبيق الإعدادات على المصنف
            workbook.Settings.GlobalizationSettings = settings;

            // إنشاء صيغة مصفوفة بالفاصل المخصص باستخدام SetArrayFormula
            worksheet.Cells["A1"].SetArrayFormula("SUM({1,2,3;4,5,6})", 1, 1);
            worksheet.Cells["A2"].Formula = "=SUM(A1)";

            // حساب الصيغ
            workbook.CalculateFormula();

            // اعرض النتيجة
            Console.WriteLine("Result of array formula calculation: " + worksheet.Cells["A2"].Value);

            // احفظ المصنف
            workbook.Save("PropertyColumnSeparatorOfFormulaArrayDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


