---
title: "FormulaSettings.ForceFullCalculation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormulaSettings. تشير إلى ما إذا كانت تحسب جميع الصيغ في كل مرة يتم فيها تشغيل عملية حساب"
type: docs
url: /ar/net/aspose.cells/formulasettings/forcefullcalculation/
---
## FormulaSettings.ForceFullCalculation property

يشير إلى ما إذا كان يحسب جميع الصيغ في كل مرة يتم فيها تشغيل حساب.

```csharp
public bool ForceFullCalculation { get; set; }
```

### ملاحظات

هذه الخاصية مخصصة فقط لحفظ الإعدادات إلى ملف جدول البيانات الناتج بحيث يمكن للتطبيقات الأخرى (مثل ms excel) أن تتصرف وفقًا لذلك عند تحميل الملف والتعامل معه. من منظور الأداء لمعظم تطبيقات المستخدمين، لا نقوم بحساب أي صيغة في المصنف تلقائيًا، بغض النظر عن القيمة التي تم تعيينها لهذه الخاصية.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyForceFullCalculationDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى إعدادات الصيغ
            FormulaSettings formulaSettings = workbook.Settings.FormulaSettings;

            // عرض خاصية ForceFullCalculation
            formulaSettings.ForceFullCalculation = true;
            Console.WriteLine($"ForceFullCalculation is set to: {formulaSettings.ForceFullCalculation}");

            // أضف بيانات تجريبية وصيغة
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // حساب الصيغ باستخدام إعداد ForceFullCalculation
            workbook.CalculateFormula();

            // أخرج النتيجة.
            Console.WriteLine($"Calculation result: {worksheet.Cells["A3"].Value}");

            // احفظ المصنف
            workbook.Save("ForceFullCalculationDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


