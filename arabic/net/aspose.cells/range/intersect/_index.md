---
title: "Range.Intersect"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. تُعيد كائن Range يمثل التقاطع المستطيل لنطاقين"
type: docs
url: /ar/net/aspose.cells/range/intersect/
---
## Range.Intersect method

تُعيد كائن [`Range`](../) يمثل التقاطع المستطيل لنطاقين.

```csharp
public Range Intersect(Range range)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نطاق | النطاق | النطاق المتقاطع. |

### قيمة الإرجاع

تُعيد كائن [`Range`](../)

### ملاحظات

إذا لم يتقاطع النطاقان، تُعيد null.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodIntersectWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            Aspose.Cells.Range range1 = cells.CreateRange("A1:A5");
            Aspose.Cells.Range range2 = cells.CreateRange("A3:A10");
            
            Aspose.Cells.Range intersectRange = range1.Intersect(range2);
            
            Console.WriteLine("Intersected range: " + intersectRange.Address);
            workbook.Save("IntersectDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


