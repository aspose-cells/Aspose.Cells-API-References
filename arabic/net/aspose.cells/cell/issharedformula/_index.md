---
title: "Cell.IsSharedFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تشير إلى ما إذا كانت صيغة الخلية جزءًا من صيغة مشتركة"
type: docs
url: /ar/net/aspose.cells/cell/issharedformula/
---
## Cell.IsSharedFormula property

يشير إلى ما إذا كانت صيغة الخلية جزءًا من صيغة مشتركة.

```csharp
public bool IsSharedFormula { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsSharedFormulaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين صيغة مشتركة في نطاق
            worksheet.Cells["B2"].Formula = "=A2*2";
            worksheet.Cells["B2"].Copy(worksheet.Cells["B3:B5"]);

            // تحقق مما إذا كانت الخلايا تحتوي على صيغة مشتركة
            Cell cellB2 = worksheet.Cells["B2"];
            Cell cellB3 = worksheet.Cells["B3"];

            Console.WriteLine("Cell B2 IsSharedFormula: " + cellB2.IsSharedFormula);
            Console.WriteLine("Cell B3 IsSharedFormula: " + cellB3.IsSharedFormula);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


