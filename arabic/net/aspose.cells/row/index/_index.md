---
title: "Row.Index"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Row. تحصل على فهرس هذا الصف"
type: docs
url: /ar/net/aspose.cells/row/index/
---
## Row.Index property

يسترجع فهرس هذا الصف.

```csharp
public int Index { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIndexDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات إلى الخلايا
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // التنقل عبر الصفوف وعرض خاصية Index
            foreach (Row row in worksheet.Cells.Rows)
            {
                Console.WriteLine($"Processing row with index: {row.Index}");
                if (row.Index > 0) // Skip header row
                {
                    Console.WriteLine($"Data in row {row.Index}: " +
                        $"{worksheet.Cells[row.Index, 0].StringValue}, " +
                        $"{worksheet.Cells[row.Index, 1].IntValue}");
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


