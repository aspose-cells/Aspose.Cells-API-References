---
title: "SignatureLine.Instructions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SignatureLine. يحصل أو يضبط النص المعروض للمستخدم عند التوقيع"
type: docs
url: /ar/net/aspose.cells.drawing/signatureline/instructions/
---
## SignatureLine.Instructions property

يحصل أو يعيّن النص المعروض للمستخدم عند توقيع.

```csharp
public string Instructions { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyInstructionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء كائن سطر توقيع
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Instructions = "Please sign here after reviewing the document.";

            // إضافة سطر التوقيع إلى ورقة العمل في الموضع (1,1)
            worksheet.Shapes.AddSignatureLine(1, 1, signatureLine);

            // احفظ المصنف
            workbook.Save("SignatureLineDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


