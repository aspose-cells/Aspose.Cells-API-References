---
title: "FormulaSettings.CalculationId"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormulaSettings. تحدد نسخة محرك الحساب المستخدم لحساب القيم في المصنف"
type: docs
url: /ar/net/aspose.cells/formulasettings/calculationid/
---
## FormulaSettings.CalculationId property

يحدد إصدار محرك الحساب المستخدم لحساب القيم في المصنف.

```csharp
public string CalculationId { get; set; }
```

### ملاحظات

هذه الخاصية مخصصة فقط لحفظ الإعدادات إلى ملف جدول البيانات الناتج بحيث يمكن للتطبيقات الأخرى (مثل ms excel) أن تتصرف وفقًا لذلك عند تحميل الملف والتعامل معه. في حالة ms excel، إذا كانت قيمة هذه الخاصية أقل من معرف محرك إعادة الحساب المرتبط بالتطبيق الذي يفتح الملف الناتج، سيعيد التطبيق حساب نتائج جميع الصيغ في هذا المصنف فورًا بعد تحميل الملف. من منظور الأداء لمعظم تطبيقات المستخدمين، لا نقوم بحساب أي صيغة في المصنف تلقائيًا، بغض النظر عن القيمة التي تم تعيينها لهذه الخاصية.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculationIdDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // تعيين صيغة تتصرف بشكل مختلف بناءً على CalculationId
            Cell cell = sheet.Cells["A1"];
            cell.Formula = "=AND(\"a\",true)";
            
            // حساب دون CalculationId (السلوك الافتراضي)
            wb.CalculateFormula();
            Console.WriteLine("Without CalculationId: " + cell.Value);
            
            // تعيين CalculationId وإعادة الحساب
            wb.Settings.FormulaSettings.CalculationId = "181029";
            wb.CalculateFormula();
            Console.WriteLine("With CalculationId 181029: " + cell.BoolValue);
        }
    }
}
```

### انظر أيضًا

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


