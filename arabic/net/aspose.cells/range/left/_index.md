---
title: "Range.Left"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Range. يحصل على المسافة بالنقاط من الحافة اليسرى للعمود A إلى الحافة اليسرى للنطاق"
type: docs
url: /ar/net/aspose.cells/range/left/
---
## Range.Left property

يحصل على المسافة، بالنقاط، من الحافة اليسرى للعمود A إلى الحافة اليسرى للنطاق.

```csharp
public double Left { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyLeftDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نطاق من B2 إلى C4
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:C4");
            
            // عرض استخدام خاصية Left
            Console.WriteLine("Range Left position: " + range.Left);
            Console.WriteLine("Range Width: " + range.Width);
            
            // حساب القيم المتوقعة بناءً على حالة الاختبار
            double expectedLeft = 64 / 96.0 * 72;
            Console.WriteLine("Expected Left position: " + expectedLeft);
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


