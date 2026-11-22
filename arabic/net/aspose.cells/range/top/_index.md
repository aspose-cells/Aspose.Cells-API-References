---
title: "Range.Top"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Range. يحصل على المسافة بالنقاط من الحافة العلوية للصف 1 إلى الحافة العلوية للنطاق"
type: docs
url: /ar/net/aspose.cells/range/top/
---
## Range.Top property

يحصل على المسافة، بالنقاط، من الحافة العلوية للصف 1 إلى الحافة العلوية للنطاق.

```csharp
public double Top { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyTopDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نطاق وضبط بعض القيم
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            range[0, 0].PutValue("Test");
            
            // عرض كيفية استخدام خاصية Top
            Console.WriteLine("Range Top position: " + range.Top);
            Console.WriteLine("Range Height: " + range.Height);
            Console.WriteLine("Range Left position: " + range.Left);
            Console.WriteLine("Range Width: " + range.Width);
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


