---
title: "SignatureLine.Signer"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SignatureLine. تحصل أو تعين المُوقّع"
type: docs
url: /ar/net/aspose.cells.drawing/signatureline/signer/
---
## SignatureLine.Signer property

يحصل أو يعيّن الموقع.

```csharp
public string Signer { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertySignerDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء سطر توقيع وتعيين خصائصه
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "john.doe@example.com";

            // إضافة سطر التوقيع إلى ورقة العمل في الصف 1، العمود 1
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

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


