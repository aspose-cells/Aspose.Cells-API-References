---
title: "Cell.IsArrayFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تشير إلى ما إذا كانت صيغة الخلية صيغة مصفوفة"
type: docs
url: /ar/net/aspose.cells/cell/isarrayformula/
---
## Cell.IsArrayFormula property

يشير إلى ما إذا كانت صيغة الخلية صيغة مصفوفة.

```csharp
public bool IsArrayFormula { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsArrayFormulaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء صيغة مصفوفة في الخلية B2
            worksheet.Cells["B2"].SetArrayFormula("SUM(A1:A10*B1:B10)", 1, 1);
            
            // تحقق مما إذا كانت الخلية تحتوي على صيغة مصفوفة
            bool isArrayFormula = worksheet.Cells["B2"].IsArrayFormula;
            
            // أخرج النتيجة.
            Console.WriteLine("Cell B2 is an array formula: " + isArrayFormula);
            
            // احفظ المصنف
            workbook.Save("IsArrayFormulaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


