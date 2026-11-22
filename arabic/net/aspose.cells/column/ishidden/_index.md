---
title: "Column.IsHidden"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Column. تشير إلى ما إذا كان العمود مخفيًا"
type: docs
url: /ar/net/aspose.cells/column/ishidden/
---
## Column.IsHidden property

يشير إلى ما إذا كان العمود مخفيًا.

```csharp
public bool IsHidden { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين عرض العمود للتوضيح
            worksheet.Cells.Columns[1].Width = 20;
            Console.WriteLine("Column 1 width before hiding: " + worksheet.Cells.Columns[1].Width);

            // إخفاء العمود
            worksheet.Cells.Columns[1].IsHidden = true;
            Console.WriteLine("Column 1 is hidden: " + worksheet.Cells.Columns[1].IsHidden);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


