---
title: "Range.GetOffset"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. يحصل على نطاق Range بالإزاحة"
type: docs
url: /ar/net/aspose.cells/range/getoffset/
---
## Range.GetOffset method

يحصل على نطاق [`Range`](../) بالإزاحة.

```csharp
public Range GetOffset(int rowOffset, int columnOffset)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowOffset | Int32 | إزاحة الصف في هذا النطاق، بدءًا من الصفر. |
| columnOffset | Int32 | إزاحة العمود في هذا النطاق، بدءًا من الصفر. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetOffsetWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // إنشاء النطاق الأولي
            Aspose.Cells.Range originalRange = cells.CreateRange("A1");
            Console.WriteLine("Original Range Address: " + originalRange.Address);
            
            // احصل على نطاق الإزاحة
            Aspose.Cells.Range offsetRange = originalRange.GetOffset(1, 1);
            Console.WriteLine("Offset Range Address: " + offsetRange.Address);
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


