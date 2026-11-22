---
title: "Row.GetCellByIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Row. احصل على الخلية بواسطة فهرس محدد في مجموعة الخلايا لهذا الصف"
type: docs
url: /ar/net/aspose.cells/row/getcellbyindex/
---
## Row.GetCellByIndex method

احصل على الخلية بواسطة فهرس محدد في مجموعة الخلايا لهذا الصف.

```csharp
public Cell GetCellByIndex(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | الفهرس (الموقع) للخلية في مجموعة الخلايا لهذا الصف. |

### قيمة الإرجاع

كائن Cell في الموقع المحدد.

### ملاحظات

للتنقل عبر جميع الخلايا بالتسلسل دون تعديل، سيؤدي استخدام [`GetEnumerator`](../getenumerator/) إلى أداء أفضل مقارنةً باستخدام هذه الطريقة للحصول على الخلية واحدةً تلو الأخرى.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetCellByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات إلى الخلايا في الصف الأول
            worksheet.Cells["A1"].PutValue("Cell A1");
            worksheet.Cells["B1"].PutValue("Cell B1");
            worksheet.Cells["C1"].PutValue("Cell C1");

            // احصل على الصف الأول
            Row row = worksheet.Cells.Rows[0];

            // عرض GetCellByIndex مع معامل Int32
            Cell cellAtIndex0 = row.GetCellByIndex(0);
            Cell cellAtIndex1 = row.GetCellByIndex(1);
            Cell cellAtIndex2 = row.GetCellByIndex(2);

            Console.WriteLine("Cell at index 0: " + cellAtIndex0.StringValue);
            Console.WriteLine("Cell at index 1: " + cellAtIndex1.StringValue);
            Console.WriteLine("Cell at index 2: " + cellAtIndex2.StringValue);

            workbook.Save("RowGetCellByIndexDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


