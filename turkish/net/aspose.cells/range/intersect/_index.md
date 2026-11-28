---
title: "Range.Intersect"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. İki aralığın dikdörtgen kesişimini temsil eden bir Range nesnesi döndürür"
type: docs
url: /tr/net/aspose.cells/range/intersect/
---
## Range.Intersect method

[`Range`](../) nesnesi, iki aralığın dikdörtgen kesişimini temsil eder.

```csharp
public Range Intersect(Range range)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aralık | Aralık | Kesişen aralık. |

### Dönüş Değeri

[`Range`](../) nesnesi döndürür

### Açıklamalar

İki aralık kesişmiyorsa, null döndürür.

### Örnekler

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

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


