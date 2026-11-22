---
title: "Cell.IsArrayHeader"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تشير إلى أن صيغة الخلية هي صيغة مصفوفة وأنها الخلية الأولى في المصفوفة"
type: docs
url: /ar/net/aspose.cells/cell/isarrayheader/
---
## Cell.IsArrayHeader property

يشير إلى أن صيغة الخلية هي صيغة مصفوفة وأنها الخلية الأولى في المصفوفة.

```csharp
public bool IsArrayHeader { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsArrayHeaderDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء صيغة مصفوفة في النطاق B2:D4
            worksheet.Cells["B2"].SetArrayFormula("=A1:A3*B1:B3", 3, 3);
            
            // تحقق واطبع خاصية IsArrayHeader
            // ملاحظة: IsArrayHeader للقراءة فقط ويتم تعيينه تلقائيًا لرؤوس صيغ المصفوفة
            Console.WriteLine("B2 IsArrayHeader: " + worksheet.Cells["B2"].IsArrayHeader);
            Console.WriteLine("B3 IsArrayHeader: " + worksheet.Cells["B3"].IsArrayHeader);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


