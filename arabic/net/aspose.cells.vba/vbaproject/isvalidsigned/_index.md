---
title: "VbaProject.IsValidSigned"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية VbaProject. تشير إلى ما إذا كانت توقيع مشروع VBA صالحًا أم لا"
type: docs
url: /ar/net/aspose.cells.vba/vbaproject/isvalidsigned/
---
## VbaProject.IsValidSigned property

يشير إلى ما إذا كانت توقيع مشروع VBA صالحًا أم لا.

```csharp
public bool IsValidSigned { get; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectPropertyIsValidSignedDemo
    {
        public static void Run()
        {
            // حمّل مصنفًا تجريبيًا مع مشروع VBA موقع
            Workbook wb = new Workbook("example.xlsm");
            
            // تحقق مما إذا كان مشروع VBA موقعًا وما إذا كانت التوقيع صالحًا
            Console.WriteLine("Is VBA Project Signed: " + wb.VbaProject.IsSigned);
            Console.WriteLine("Is Signature Valid: " + wb.VbaProject.IsValidSigned);

            // احفظ وأعد التحميل للتحقق من بقاء التوقيع
            MemoryStream ms = new MemoryStream();
            wb.Save(ms, SaveFormat.Excel97To2003);
            
            Workbook validateWb = new Workbook(ms);
            Console.WriteLine("After Reload - Is VBA Project Signed: " + validateWb.VbaProject.IsSigned);
            Console.WriteLine("After Reload - Is Signature Valid: " + validateWb.VbaProject.IsValidSigned);
        }
    }
}
```

### انظر أيضًا

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


