---
title: "SignatureLine.Id"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SignatureLine. يحصل أو يضبط المعرف لهذا سطر التوقيع"
type: docs
url: /ar/net/aspose.cells.drawing/signatureline/id/
---
## SignatureLine.Id property

يحصل أو يعيّن المعرف لهذا خط التوقيع.

```csharp
public Guid Id { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyIdDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء كائن سطر توقيع
            SignatureLine signatureLine = new SignatureLine();
            Guid signatureId = Guid.NewGuid();
            signatureLine.Id = signatureId;
            
            // إضافة سطر التوقيع إلى ورقة العمل في الموضع (1,1)
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

            // عرض معرف سطر التوقيع
            Console.WriteLine("Signature Line ID: " + signatureLine.Id);
        }
    }
}
```

### انظر أيضًا

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


