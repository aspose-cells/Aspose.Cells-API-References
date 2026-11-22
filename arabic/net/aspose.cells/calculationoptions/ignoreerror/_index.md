---
title: "CalculationOptions.IgnoreError"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CalculationOptions. يوضح ما إذا كان يجب تجاهل الأخطاء التي تحدث أثناء حساب الصيغ. قد يكون الخطأ نتيجة دالة غير مدعومة أو روابط خارجية إلخ. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/calculationoptions/ignoreerror/
---
## CalculationOptions.IgnoreError property

يشير إلى ما إذا كان يجب تجاهل الأخطاء التي تم مواجهتها أثناء حساب الصيغ. قد يكون الخطأ دالة غير مدعومة أو روابط خارجية، إلخ. القيمة الافتراضية هي true.

```csharp
public bool IgnoreError { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyIgnoreErrorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة نطاق مسمى غير موجود لتوضيح معالجة الأخطاء
            worksheet.Cells["A1"].Formula = "=NONEXISTENTNAME()";
            
            // حساب مع IgnoreError = false (سيرمي خطأ)
            try
            {
                workbook.CalculateFormula(new CalculationOptions() { IgnoreError = false });
                Console.WriteLine("Calculation completed without ignoring errors");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error occurred (expected): " + ex.Message);
            }

            // حساب مع IgnoreError = true (سيُقمع الخطأ)
            try
            {
                workbook.CalculateFormula(new CalculationOptions() { IgnoreError = true });
                Console.WriteLine("Calculation completed while ignoring errors");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error occurred (unexpected): " + ex.Message);
            }
        }
    }
}
```

### انظر أيضًا

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


