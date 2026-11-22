---
title: "CalculationOptions.UserSpecifiedRefreshDynamicArrayFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CalculationOptions. يوضح ما إذا كان المستخدم قد حدد صراحة سلوك تحديث صيغ المصفوفة الديناميكية قبل حساب الصيغ المحددة"
type: docs
url: /ar/net/aspose.cells/calculationoptions/userspecifiedrefreshdynamicarrayformula/
---
## CalculationOptions.UserSpecifiedRefreshDynamicArrayFormula property

يشير إلى ما إذا كان المستخدم قد حدد صراحة سلوك تحديث صيغ المصفوفة الديناميكية قبل حساب الصيغ المحددة.

```csharp
public bool UserSpecifiedRefreshDynamicArrayFormula { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationOptionsPropertyUserSpecifiedRefreshDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إنشاء ورقة عمل نموذجية
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات لجعل المثال ذو معنى
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // إنشاء كائن CalculationOptions
                CalculationOptions options = new CalculationOptions();

                // عرض القيمة الحالية لخاصية UserSpecifiedRefreshDynamicArrayFormula
                Console.WriteLine("UserSpecifiedRefreshDynamicArrayFormula value: " +
                    options.UserSpecifiedRefreshDynamicArrayFormula);

                // إظهار كيف تؤثر الخاصية على السلوك
                Console.WriteLine("UserSpecifiedRefreshDynamicArrayFormula has been demonstrated");

                // حفظ النتيجة
                workbook.Save("UserSpecifiedRefreshDynamicArrayFormulaDemo.xlsx");
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


