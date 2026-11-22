---
title: "Column.Index"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Column. تحصل على فهرس هذا العمود"
type: docs
url: /ar/net/aspose.cells/column/index/
---
## Column.Index property

يحصل على فهرس هذا العمود.

```csharp
public int Index { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyIndexDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بعض البيانات إلى الأعمدة
            worksheet.Cells["A1"].PutValue("Column 1");
            worksheet.Cells["B1"].PutValue("Column 2");
            worksheet.Cells["C1"].PutValue("Column 3");
            
            // الحصول على مجموعة الأعمدة
            ColumnCollection columns = worksheet.Cells.Columns;
            
            // توضيح خاصية Index
            Console.WriteLine("Column Indices:");
            for (int i = 0; i < columns.Count; i++)
            {
                Column column = columns[i];
                Console.WriteLine($"Column {column.Index}: {worksheet.Cells[0, column.Index].StringValue}");
            }
            
            // الوصول إلى العمود بواسطة الفهرس
            Column columnB = columns[1]; // B column (index 1)
            Console.WriteLine($"\nAccessed by index 1: {worksheet.Cells[0, columnB.Index].StringValue}");
            
            // تعديل عرض العمود باستخدام الفهرس
            columns[2].Width = 30; // C column (index 2)
            Console.WriteLine($"\nColumn C width set to: {columns[2].Width}");
        }
    }
}
```

### انظر أيضًا

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


