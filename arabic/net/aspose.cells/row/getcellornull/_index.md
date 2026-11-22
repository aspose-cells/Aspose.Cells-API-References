---
title: "Row.GetCellOrNull"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Row. تحصل على الخلية أو قيمة null في الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/row/getcellornull/
---
## Row.GetCellOrNull method

يسترجع الخلية أو null في الفهرس المحدد.

```csharp
public Cell GetCellOrNull(int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | Int32 | فهرس العمود |

### قيمة الإرجاع

يرجع كائن الخلية إذا كانت الخلية موجودة. أو يرجع null إذا لم يكن كائن الخلية موجودًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetCellOrNullWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // أضف بيانات تجريبية
            ws.Cells["A1"].PutValue("Header1");
            ws.Cells["B1"].PutValue("Header2");
            ws.Cells["A2"].PutValue(100);
            ws.Cells["B2"].PutValue(200);

            // احصل على الصف الأول
            Row row = ws.Cells.Rows[0];

            // عرض GetCellOrNull مع معامل Int32
            for (int colIndex = 0; colIndex < 2; colIndex++)
            {
                Cell cell = row.GetCellOrNull(colIndex);
                if (cell != null)
                {
                    Console.WriteLine($"Cell at column {colIndex}: {cell.StringValue}");
                }
                else
                {
                    Console.WriteLine($"Cell at column {colIndex} is null");
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


