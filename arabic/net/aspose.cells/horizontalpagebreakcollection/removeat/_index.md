---
title: "HorizontalPageBreakCollection.RemoveAt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة HorizontalPageBreakCollection. تزيل عنصر HPageBreak عند اسم محدد"
type: docs
url: /ar/net/aspose.cells/horizontalpagebreakcollection/removeat/
---
## HorizontalPageBreakCollection.RemoveAt method

يزيل عنصر HPageBreak عند اسم محدد.

```csharp
public void RemoveAt(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | فهرس العنصر، يبدأ من الصفر. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            worksheet.HorizontalPageBreaks.Add(15);
            
            worksheet.HorizontalPageBreaks.RemoveAt(0);
            
            workbook.Save("HorizontalPageBreakCollectionExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


