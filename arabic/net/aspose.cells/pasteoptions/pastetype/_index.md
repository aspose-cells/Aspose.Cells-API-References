---
title: "PasteOptions.PasteType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PasteOptions. نوع اللصق الخاص"
type: docs
url: /ar/net/aspose.cells/pasteoptions/pastetype/
---
## PasteOptions.PasteType property

نوع اللصق الخاص.

```csharp
public PasteType PasteType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyPasteTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين قيمة المصدر
            worksheet.Cells["A1"].PutValue("SourceValue");

            // إنشاء نطاقات بأسماء الأنواع المؤهلة بالكامل
            Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1");
            Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("B1:D3");

            // نسخ مع PasteType.All
            targetRange.Copy(sourceRange, new PasteOptions() { PasteType = PasteType.All });

            // إخراج النتائج
            Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue);
            Console.WriteLine("B1: " + worksheet.Cells["B1"].StringValue);
            Console.WriteLine("C2: " + worksheet.Cells["C2"].StringValue);
            Console.WriteLine("D3: " + worksheet.Cells["D3"].StringValue);
        }
    }
}
```

### انظر أيضًا

* enum [PasteType](../../pastetype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


