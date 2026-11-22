---
title: "FormulaSettings.CalculateOnSave"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormulaSettings. تشير إلى ما إذا كان يجب إعادة حساب المصنف قبل حفظ المستند عندما يكون في وضع الحساب اليدوي"
type: docs
url: /ar/net/aspose.cells/formulasettings/calculateonsave/
---
## FormulaSettings.CalculateOnSave property

يشير إلى ما إذا كان يجب إعادة حساب المصنف قبل حفظ المستند، عند وضع الحساب اليدوي.

```csharp
public bool CalculateOnSave { get; set; }
```

### ملاحظات

هذه الخاصية مخصصة فقط لحفظ الإعدادات إلى ملف جدول البيانات الناتج بحيث يمكن للتطبيقات الأخرى (مثل ms excel) أن تتصرف وفقًا لذلك عند تحميل الملف والتعامل معه. من منظور الأداء لمعظم تطبيقات المستخدمين، لا نقوم بحساب أي صيغة في المصنف تلقائيًا، بغض النظر عن القيمة التي تم تعيينها لهذه الخاصية.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculateOnSaveDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل وإضافة بعض البيانات
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // تعطيل CalculateOnSave (القيمة الافتراضية هي false)
            workbook.Settings.FormulaSettings.CalculateOnSave = false;
            
            // حفظ دون حساب الصيغ
            workbook.Save("output_without_calculation.xlsx");

            // تمكين CalculateOnSave
            workbook.Settings.FormulaSettings.CalculateOnSave = true;
            
            // حفظ مع حساب الصيغ
            workbook.Save("output_with_calculation.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


