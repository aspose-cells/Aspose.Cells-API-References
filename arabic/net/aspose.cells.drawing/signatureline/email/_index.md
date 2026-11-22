---
title: "SignatureLine.Email"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SignatureLine. يحصل أو يضبط البريد الإلكتروني للمُوقّع"
type: docs
url: /ar/net/aspose.cells.drawing/signatureline/email/
---
## SignatureLine.Email property

يحصل أو يعيّن البريد الإلكتروني للمغني.

```csharp
public string Email { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyEmailDemo
    {
        public static void Run()
        {
            // إنشاء سطر توقيع جديد
            SignatureLine signatureLine = new SignatureLine();
            
            // تعيين خصائص سطر التوقيع بما في ذلك البريد الإلكتروني
            signatureLine.Signer = "Simon Zhao";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "Simon.Zhao@aspose.com";
            signatureLine.IsLine = true;
            signatureLine.ShowSignedDate = true;
            
            // عرض خاصية البريد الإلكتروني
            Console.WriteLine("Signer Email: " + signatureLine.Email);
        }
    }
}
```

### انظر أيضًا

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


