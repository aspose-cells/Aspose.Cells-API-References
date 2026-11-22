---
title: "GlobalizationSettings.RowSeparatorOfFormulaArray"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GlobalizationSettings. يحصل على الفاصل للصفوف في بيانات المصفوفة في الصيغة"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/rowseparatorofformulaarray/
---
## GlobalizationSettings.RowSeparatorOfFormulaArray property

يحصل على الفاصل للصفوف في بيانات المصفوفة في الصيغة.

```csharp
public virtual char RowSeparatorOfFormulaArray { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyRowSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد بإعدادات عولمة مخصصة
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى نسخة إعدادات العولمة المخصصة
            CustomGlobalizationSettings settings = (CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings;

            // عرض القيمة الحالية لـ RowSeparatorOfFormulaArray
            Console.WriteLine("Current RowSeparatorOfFormulaArray value: " + settings.RowSeparatorOfFormulaArray);

            // إنشاء صيغة مصفوفة باستخدام الفاصل الصفّي المخصص
            Cell cell = worksheet.Cells["A1"];
            cell.Formula = "=SUM({1,2|3,4})"; // Uses '|' as row separator

            // احسب الصيغة لتوضيح التحليل الصحيح
            workbook.CalculateFormula();

            // عرض النتائج
            Console.WriteLine("Array formula using custom separator: " + cell.Formula);
            Console.WriteLine("Calculated result: " + cell.Value);

            // احفظ المصنف
            workbook.Save("PropertyRowSeparatorOfFormulaArrayDemo.xlsx");
        }
    }

    // تنفيذ مخصص لـ GlobalizationSettings يتجاوز الفاصل الصفّي
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override char RowSeparatorOfFormulaArray => '|';
    }
}
```

### انظر أيضًا

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


