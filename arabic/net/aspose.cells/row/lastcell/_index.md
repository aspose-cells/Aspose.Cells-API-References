---
title: "Row.LastCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Row. تحصل على كائن الخلية الأخيرة في الصف"
type: docs
url: /ar/net/aspose.cells/row/lastcell/
---
## Row.LastCell property

يسترجع آخر كائن خلية في الصف.

```csharp
public Cell LastCell { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyLastCellDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("First");
            worksheet.Cells["B1"].PutValue("Second");
            worksheet.Cells["C1"].PutValue("Last");

            // احصل على الصف الأول
            Row row = worksheet.Cells.Rows[0];

            // الوصول إلى الخلية الأخيرة في الصف
            Cell lastCell = row.LastCell;
            
            // إخراج قيمة الخلية الأخيرة
            Console.WriteLine("Last cell value: " + lastCell.Value);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


