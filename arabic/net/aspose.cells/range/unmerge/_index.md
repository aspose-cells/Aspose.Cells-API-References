---
title: "Range.UnMerge"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. تلغي دمج الخلايا المدمجة في هذا النطاق"
type: docs
url: /ar/net/aspose.cells/range/unmerge/
---
## Range.UnMerge method

يفك دمج الخلايا المدمجة في هذا النطاق.

```csharp
public void UnMerge()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodUnMergeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // دمج الخلايا من B2 إلى D4
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2", "D4");
            range.Merge();
            
            // تحقق مما إذا كانت الخلية B2 مدمجة قبل إلغاء الدمج
            Console.WriteLine("Before UnMerge - Is B2 merged? " + worksheet.Cells["B2"].IsMerged);
            
            // إلغاء دمج النطاق
            range.UnMerge();
            
            // تحقق مما إذا كانت الخلية B2 مدمجة بعد إلغاء الدمج
            Console.WriteLine("After UnMerge - Is B2 merged? " + worksheet.Cells["B2"].IsMerged);
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


