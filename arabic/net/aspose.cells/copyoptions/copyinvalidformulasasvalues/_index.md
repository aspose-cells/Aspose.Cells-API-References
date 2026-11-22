---
title: "CopyOptions.CopyInvalidFormulasAsValues"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CopyOptions. إذا كانت الصيغة غير صالحة للوجهة، يتم نسخ القيم فقط."
type: docs
url: /ar/net/aspose.cells/copyoptions/copyinvalidformulasasvalues/
---
## CopyOptions.CopyInvalidFormulasAsValues property

إذا كانت الصيغة غير صالحة للوجهة المستهدفة، يتم نسخ القيم فقط.

```csharp
public bool CopyInvalidFormulasAsValues { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyCopyInvalidFormulasAsValuesDemo
    {
        public static void Run()
        {
            // إنشاء مصنف مصدر مع ورقة عمل عينة
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            
            // إضافة صيغة قد تكون غير صالحة في بعض السياقات
            srcSheet.Cells["A1"].Formula = "=1/0"; // Division by zero - invalid formula
            srcSheet.Cells["A2"].Value = "Valid Data";

            // إنشاء دفتر عمل هدف
            Workbook destWorkbook = new Workbook();
            
            // تعيين خيارات النسخ لتحويل الصيغ غير الصالحة إلى قيم
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.CopyInvalidFormulasAsValues = true;

            // نسخ ورقة العمل باستخدام الخيارات
            destWorkbook.Worksheets[0].Copy(srcSheet, copyOptions);

            // تحقق من النتائج
            Console.WriteLine("A1 (invalid formula copied as value): " + 
                destWorkbook.Worksheets[0].Cells["A1"].Value); // Should show #DIV/0! as value
            Console.WriteLine("A2 (valid data): " + 
                destWorkbook.Worksheets[0].Cells["A2"].Value); // Should show "Valid Data"
        }
    }
}
```

### انظر أيضًا

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


