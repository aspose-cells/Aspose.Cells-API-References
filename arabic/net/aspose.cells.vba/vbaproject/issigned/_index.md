---
title: "VbaProject.IsSigned"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VbaProject. تشير إلى ما إذا كان كود VBA موقعًا أم لا"
type: docs
url: /ar/net/aspose.cells.vba/vbaproject/issigned/
---
## VbaProject.IsSigned property

يشير إلى ما إذا كان VBAcode موقعًا أم لا.

```csharp
public bool IsSigned { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIsSignedDemo
    {
        public static void Run()
        {
            // تحميل ملف Excel تجريبي يحتوي على مشروع VBA
            Workbook workbook = new Workbook("example.xlsm");
            
            // التحقق مما إذا كان مشروع VBA موقعًا
            if (workbook.VbaProject.IsSigned)
            {
                Console.WriteLine("VBA project is signed.");
                Console.WriteLine("Signature is valid: " + workbook.VbaProject.IsValidSigned);
            }
            else
            {
                Console.WriteLine("VBA project is not signed.");
            }
        }
    }
}
```

### انظر أيضًا

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


