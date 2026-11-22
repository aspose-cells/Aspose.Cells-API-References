---
title: "Cells.CheckCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحصل على عنصر Cell أو null في مؤشر صف الخلية المحدد ومؤشر العمود المحدد"
type: docs
url: /ar/net/aspose.cells/cells/checkcell/
---
## Cells.CheckCell method

يحصل على عنصر [`Cell`](../../cell/) أو null في مؤشر صف الخلية المحدد ومؤشر العمود المحدد.

```csharp
public Cell CheckCell(int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف |
| عمود | Int32 | فهرس العمود |

### قيمة الإرجاع

إرجاع كائن Cell إذا كان كائن Cell موجودًا. إرجاع null إذا لم تكن الخلية موجودة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckCellWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين القيم في الخلايا
            cells[0, 0].PutValue("Hello");
            cells[1, 1].PutValue(123);
            cells[2, 2].PutValue(DateTime.Now);

            // تحقق من الخلايا باستخدام طريقة CheckCell مع معلمات Int32
            Cell cell1 = cells.CheckCell(0, 0);
            Console.WriteLine("Cell A1 value: " + cell1.StringValue);

            Cell cell2 = cells.CheckCell(1, 1);
            Console.WriteLine("Cell B2 value: " + cell2.StringValue);

            Cell cell3 = cells.CheckCell(2, 2);
            Console.WriteLine("Cell C3 value: " + cell3.StringValue);

            // تحقق من خلية غير موجودة (ستُعيد null)
            Cell cell4 = cells.CheckCell(10, 10);
            if (cell4 == null)
            {
                Console.WriteLine("Cell K11 doesn't exist (as expected)");
            }
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


