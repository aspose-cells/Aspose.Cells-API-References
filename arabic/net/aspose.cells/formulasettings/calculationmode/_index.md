---
title: "FormulaSettings.CalculationMode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormulaSettings. يحصل على أو يضبط وضع حساب المصنف في MS Excel"
type: docs
url: /ar/net/aspose.cells/formulasettings/calculationmode/
---
## FormulaSettings.CalculationMode property

يحصل أو يضبط وضع حساب المصنف في MS Excel.

```csharp
public CalcModeType CalculationMode { get; set; }
```

### ملاحظات

هذه الخاصية مخصصة فقط لحفظ الإعدادات إلى ملف الجدول الناتج بحيث يمكن للتطبيقات الأخرى (مثل ms excel) أن تتصرف وفقًا لذلك عند تحميل الملف الناتج ومعالجته. لأسباب الأداء في معظم تطبيقات المستخدم، لا نقوم بحساب أي صيغة في المصنف تلقائيًا، بغض النظر عن الوضع الذي تم ضبطه لهذه الخاصية. إذا كان المستخدم يحتاج إلى حساب الصيغ، يرجى دائمًا استدعاء الطرق على الكائنات المختلفة حسب المتطلبات: [`CalculateFormula`](../../workbook/calculateformula/), [`CalculateFormula`](../../worksheet/calculateformula/), [`Calculate`](../../cell/calculate/), ...إلخ.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaSettingsPropertyCalculationModeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // ضبط وضع الحساب إلى AutomaticExceptTable
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.AutomaticExceptTable;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);

            // تغيير وضع الحساب إلى Manual
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Manual;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);

            // إعادة الضبط إلى الوضع الافتراضي Automatic
            workbook.Settings.FormulaSettings.CalculationMode = CalcModeType.Automatic;
            Console.WriteLine("Calculation Mode: " + workbook.Settings.FormulaSettings.CalculationMode);
        }
    }
}
```

### انظر أيضًا

* enum [CalcModeType](../../calcmodetype/)
* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


