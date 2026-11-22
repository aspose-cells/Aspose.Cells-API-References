---
title: "CalculationOptions.RefreshDynamicArrayFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CalculationOptions. تشير إلى ما إذا كان يجب تحديث صيغ المصفوفة الديناميكية قبل حساب الصيغ"
type: docs
url: /ar/net/aspose.cells/calculationoptions/refreshdynamicarrayformula/
---
## CalculationOptions.RefreshDynamicArrayFormula property

يشير إلى ما إذا كان يجب تحديث صيغ المصفوفة الديناميكية قبل حساب الصيغ.

```csharp
public bool RefreshDynamicArrayFormula { get; set; }
```

### ملاحظات

إذا تم تحديد هذه الخاصية صراحةً، فسيتم استخدام القيمة المحددة لتحديد ما إذا كان يجب تحديث صيغ المصفوفة الديناميكية. وإلا ([`UserSpecifiedRefreshDynamicArrayFormula`](../userspecifiedrefreshdynamicarrayformula/) هو خاطئ)، تعتمد القيمة الافتراضية لها على نوع الصيغ التي تحتاج إلى حسابها: لحساب صيغ المصنف، مثل [`CalculateFormula`](../../workbook/calculateformula/)، ستُعتبر هذه الخاصية صحيحة. في الحالات الأخرى، مثل [`Calculate`](../../cell/calculate/) أو [`CalculateFormula`](../../worksheet/calculateformula/)، ستُعتبر هذه الخاصية خاطئة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationOptionsPropertyRefreshDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف صيغة مصفوفة ديناميكية لتوضيح الوظيفة
            worksheet.Cells["A1"].Value = 1;
            worksheet.Cells["A2"].Value = 2;
            worksheet.Cells["A3"].Value = 3;
            worksheet.Cells["B1"].Formula = "=A1:A3"; // Dynamic array formula

            // إنشاء كائن CalculationOptions
            CalculationOptions options = new CalculationOptions();

            try
            {
                // عرض القيمة الافتراضية لـ RefreshDynamicArrayFormula
                Console.WriteLine("Default RefreshDynamicArrayFormula value: " + options.RefreshDynamicArrayFormula);

                // عيّن الخاصية إلى true لتحديث صيغ المصفوفة الديناميكية
                options.RefreshDynamicArrayFormula = true;
                Console.WriteLine("After setting to true: " + options.RefreshDynamicArrayFormula);

                // احسب الصيغ باستخدام الخيارات المحددة
                workbook.CalculateFormula(options);

                // اعرض النتيجة المحسوبة
                Console.WriteLine("Dynamic array formula result: " + worksheet.Cells["B1"].Value);

                // احفظ المصنف
                workbook.Save("RefreshDynamicArrayFormulaDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


