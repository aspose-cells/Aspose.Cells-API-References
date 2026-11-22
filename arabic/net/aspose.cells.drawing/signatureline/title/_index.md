---
title: "SignatureLine.Title"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SignatureLine. يحصل أو يضبط عنوان المُوقّع"
type: docs
url: /ar/net/aspose.cells.drawing/signatureline/title/
---
## SignatureLine.Title property

يحصل أو يعيّن لقب المغني.

```csharp
public string Title { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyTitleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء سطر توقيع وتعيين عنوانه
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Title = "Development Lead";

            // إضافة سطر التوقيع إلى أشكال ورقة العمل مع معلمات الموضع
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

            // إخراج العنوان لإظهار أنه تم تعيين الخاصية
            Console.WriteLine("Signature Line Title: " + signatureLine.Title);
        }
    }
}
```

### انظر أيضًا

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


