---
title: "CopyOptions.ExtendToAdjacentRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CopyOptions. تشير إلى ما إذا كان يتم توسيع النطاقات عند نسخ النطاق إلى نطاق مجاور"
type: docs
url: /ar/net/aspose.cells/copyoptions/extendtoadjacentrange/
---
## CopyOptions.ExtendToAdjacentRange property

يشير إلى ما إذا كان يتم توسيع النطاقات عند نسخ النطاق إلى نطاق مجاور.

```csharp
public bool ExtendToAdjacentRange { get; set; }
```

### ملاحظات

إذا كان true، يتم توسيع نطاق الارتباط التشعبي فقط، دون إضافة ارتباط تشعبي جديد عند نسخ الارتباطات التشعبية إلى الصفوف المجاورة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyExtendToAdjacentRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // إضافة ارتباط تشعبي إلى الخلية A1
            ws.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
            
            // إنشاء خيارات النسخ وتعيين ExtendToAdjacentRange إلى true
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.ExtendToAdjacentRange = true;

            // نسخ الصف 0 إلى الصف 1 باستخدام خيارات النسخ
            ws.Cells.CopyRows(ws.Cells, 0, 1, 1, copyOptions);

            // تحقق من أن الارتباط التشعبي تم توسيعه إلى النطاق المجاور
            Console.WriteLine("Hyperlink count after copy: " + ws.Hyperlinks.Count);
        }
    }
}
```

### انظر أيضًا

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


