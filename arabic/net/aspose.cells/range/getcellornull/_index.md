---
title: "Range.GetCellOrNull"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. الحصول على كائن Cell أو null في هذا النطاق"
type: docs
url: /ar/net/aspose.cells/range/getcellornull/
---
## Range.GetCellOrNull method

يحصل على كائن [`Cell`](../../cell/) أو null في هذا النطاق.

```csharp
public Cell GetCellOrNull(int rowOffset, int columnOffset)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowOffset | Int32 | إزاحة الصف في هذا النطاق، بدءًا من الصفر. |
| columnOffset | Int32 | إزاحة العمود في هذا النطاق، بدءًا من الصفر. |

### قيمة الإرجاع

[`Cell`](../../cell/) object.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodGetCellOrNullWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نطاق
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");
            
            // ملء بعض البيانات في النطاق
            range[0, 0].PutValue("Cell A1");
            range[0, 1].PutValue("Cell B1");
            range[1, 0].PutValue("Cell A2");
            
            // توضيح GetCellOrNull باستخدام معلمات Int32
            Cell cell1 = range.GetCellOrNull(0, 0);
            Console.WriteLine("Cell (0,0): " + (cell1 != null ? cell1.StringValue : "null"));
            
            Cell cell2 = range.GetCellOrNull(1, 1);
            Console.WriteLine("Cell (1,1): " + (cell2 != null ? cell2.StringValue : "null"));
            
            // حاول الحصول على خلية خارج النطاق (يجب أن تُرجع null)
            Cell cell3 = range.GetCellOrNull(2, 0);
            Console.WriteLine("Cell (2,0): " + (cell3 != null ? cell3.StringValue : "null"));
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


