---
title: "Cell.IsFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تمثل ما إذا كانت الخلية المحددة تحتوي على صيغة"
type: docs
url: /ar/net/aspose.cells/cell/isformula/
---
## Cell.IsFormula property

يمثل ما إذا كانت الخلية المحددة تحتوي على صيغة.

```csharp
public bool IsFormula { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsFormulaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة صيغة إلى الخلية A1
            worksheet.Cells["A1"].Formula = "=1+2";
            
            // إضافة قيمة عادية إلى الخلية A2
            worksheet.Cells["A2"].PutValue("Test");
            
            // تحقق مما إذا كانت الخلايا تحتوي على صيغ
            Console.WriteLine("A1 is formula: " + worksheet.Cells["A1"].IsFormula);
            Console.WriteLine("A2 is formula: " + worksheet.Cells["A2"].IsFormula);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


