---
title: "CellArea.CompareTo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellArea. قارن كائنين CellArea وفقًا للزاوية العليا اليسرى الخاصة بهما."
type: docs
url: /ar/net/aspose.cells/cellarea/compareto/
---
## CellArea.CompareTo method

قارن كائنين من CellArea وفقًا للزاوية العلوية اليسرى.

```csharp
public int CompareTo(object obj)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | Object |  |

### قيمة الإرجاع

إذا كانت الزاويتان في صفوف مختلفة، فقم بمقارنة فهرس الصف الخاص بهما. وإلا قارن فهرس العمود. إذا كانت الزاويتان متطابقتين، فسيتم إرجاع 0.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCompareToWithObjectDemo
    {
        public static void Run()
        {
            // إنشاء كائنين CellArea للمقارنة.
            CellArea ca1 = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            object ca2 = new CellArea { StartRow = 0, EndRow = 5, StartColumn = 0, EndColumn = 5 };

            // عرض طريقة CompareTo مع معامل Object.
            int comparisonResult = ca1.CompareTo(ca2);
            Console.WriteLine($"Comparison result: {comparisonResult}");

            // إنشاء مقارنة أخرى بمناطق متساوية.
            object ca3 = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            comparisonResult = ca1.CompareTo(ca3);
            Console.WriteLine($"Comparison result with equal areas: {comparisonResult}");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


