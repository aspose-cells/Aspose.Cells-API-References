---
title: "FormulaParseOptions.CheckAddIn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormulaParseOptions. ما إذا كان سيتم فحص الإضافات في الروابط الخارجية الموجودة لدفتر العمل الحالي لوظيفة معرفة من قبل المستخدم بدون رابط خارجي. القيمة الافتراضية هي true. إذا طابقت وظيفة المستخدم إحدى الإضافات في الروابط الخارجية الموجودة فسيتم اعتبارها الإضافة"
type: docs
url: /ar/net/aspose.cells/formulaparseoptions/checkaddin/
---
## FormulaParseOptions.CheckAddIn property

ما إذا كان يتم فحص الإضافات في الروابط الخارجية الموجودة لدفتر العمل الحالي للدالة المعرفة من قبل المستخدم دون رابط خارجي. القيمة الافتراضية هي true (إذا تطابقت الدالة المعرفة من قبل المستخدم مع إحدى الإضافات في الروابط الخارجية الموجودة، فسيتم اعتبارها الإضافة).

```csharp
public bool CheckAddIn { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormulaParseOptionsPropertyCheckAddInDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // تسجيل وظيفة الإضافة
            wb.Worksheets.RegisterAddInFunction("Test.xlam", "TEST_UDF", false);

            // بدون CheckAddIn=false - سيتم تحويل الصيغة إلى تنسيق الإضافة
            cells["A1"].SetFormula("=TEST_UDF()", new FormulaParseOptions());
            Console.WriteLine("A1 Formula (CheckAddIn=true): " + cells["A1"].Formula);

            // مع CheckAddIn=false - تظل الصيغة دون تغيير
            cells["A2"].SetFormula("=TEST_UDF()", new FormulaParseOptions() { CheckAddIn = false });
            Console.WriteLine("A2 Formula (CheckAddIn=false): " + cells["A2"].Formula);
        }
    }
}
```

### انظر أيضًا

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


