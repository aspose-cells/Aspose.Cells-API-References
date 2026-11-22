---
title: "GlobalizationSettings.ColumnSeparatorOfFormulaArray"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية GlobalizationSettings. تحصل على الفاصل للعناصر في صفوف البيانات بالمصفوفات في الصيغة"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/columnseparatorofformulaarray/
---
## GlobalizationSettings.ColumnSeparatorOfFormulaArray property

يحصل على الفاصل للعناصر في بيانات صف المصفوفة في الصيغة.

```csharp
public virtual char ColumnSeparatorOfFormulaArray { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsPropertyColumnSeparatorOfFormulaArrayDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء إعدادات تعميم مخصصة مع تجاوز فاصل العمود
            var globalizationSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = globalizationSettings;

            // عرض قيمة فاصل العمود الحالية
            Console.WriteLine("Current ColumnSeparatorOfFormulaArray value: " +
                globalizationSettings.ColumnSeparatorOfFormulaArray);

            // إنشاء صيغة مصفوفة باستخدام الفاصل المخصص
            Cell cell = worksheet.Cells["A1"];
            cell.SetArrayFormula("=SUM({1;2;3;4})", 1, 1); // Uses custom ';' column separator

            // تحقق من تخزين الصيغة (ستظهر الفواصل المنقوطة في سلسلة الصيغة الفعلية)
            Console.WriteLine("Stored array formula: " + cell.Formula);

            // حفظ المصنف المعدل
            workbook.Save("PropertyColumnSeparatorOfFormulaArrayDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override char ColumnSeparatorOfFormulaArray => ';';
        }
    }
}
```

### انظر أيضًا

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


