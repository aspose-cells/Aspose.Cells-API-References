---
title: "UnionRange.Ranges"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية UnionRange. تحصل على جميع نطاقات الاتحاد"
type: docs
url: /ar/net/aspose.cells/unionrange/ranges/
---
## UnionRange.Ranges property

يحصل على جميع نطاقات الاتحاد.

```csharp
public Range[] Ranges { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class UnionRangePropertyRangesDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            Aspose.Cells.Range r1 = cells.CreateRange("B1:C10");
            Aspose.Cells.Range r2 = cells.CreateRange("C2:D10");
            
            UnionRange unionRange = r1.UnionRanges(new Aspose.Cells.Range[] { r2 });
            
            Console.WriteLine("UnionRange contains {0} ranges:", unionRange.RangeCount);
            for (int i = 0; i < unionRange.RangeCount; i++)
            {
                Console.WriteLine("Range {0}: {1}", i + 1, unionRange.Ranges[i].Address);
            }
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


