---
title: "SignatureLine.IsLine"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SignatureLine. تشير إلى ما إذا كان سطر توقيع"
type: docs
url: /ar/net/aspose.cells.drawing/signatureline/isline/
---
## SignatureLine.IsLine property

يشير إلى ما إذا كان خط توقيع.

```csharp
public bool IsLine { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertyIsLineDemo
    {
        public static void Run()
        {
            // إنشاء مثال سطر توقيع
            SignatureLine signature = new SignatureLine();
            
            // تعيين IsLine إلى true
            signature.IsLine = true;
            
            // التحقق وعرض استخدام IsLine
            if (signature.IsLine)
            {
                Console.WriteLine("Signature line is active.");
            }
            
            // تبديل حالة IsLine
            signature.IsLine = false;
            
            if (!signature.IsLine)
            {
                Console.WriteLine("Signature line is now inactive.");
            }
        }
    }
}
```

### انظر أيضًا

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


