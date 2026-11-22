---
title: "Range.FirstColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Range. تحصل على فهرس العمود الأول في النطاق"
type: docs
url: /ar/net/aspose.cells/range/firstcolumn/
---
## Range.FirstColumn property

يحصل على فهرس العمود الأول في النطاق.

```csharp
public int FirstColumn { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyFirstColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات نموذجية
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);

            // إنشاء نطاق
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "B2");

            // توضيح خاصية FirstColumn
            Console.WriteLine("First column index of range: " + range.FirstColumn);

            // استخدم FirstColumn للوصول إلى الخلايا في العمود الأول من النطاق
            for (int i = 0; i < range.RowCount; i++)
            {
                Cell cell = range[i, 0]; // Access first column (index 0) of the range
                Console.WriteLine($"Cell[{i},0] value: {cell.StringValue}");
            }

            // احفظ المصنف
            workbook.Save("RangeFirstColumnDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


