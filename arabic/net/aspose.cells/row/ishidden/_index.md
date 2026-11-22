---
title: "Row.IsHidden"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Row. تشير إلى ما إذا كان الصف مخفيًا"
type: docs
url: /ar/net/aspose.cells/row/ishidden/
---
## Row.IsHidden property

يشير إلى ما إذا كان الصف مخفيًا.

```csharp
public bool IsHidden { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // أضف بيانات تجريبية
            for (int i = 0; i < 10; i++)
            {
                cells[$"A{i + 1}"].PutValue($"Row {i + 1}");
            }

            // إخفاء بعض الصفوف
            cells.HideRow(2);  // Row 3 (0-based index 2)
            cells.HideRow(5);  // Row 6 (0-based index 5)
            cells.HideRow(8);  // Row 9 (0-based index 8)

            // تحقق وعرض حالة IsHidden لكل صف
            for (int i = 0; i < 10; i++)
            {
                bool isHidden = cells.Rows[i].IsHidden;
                Console.WriteLine($"Row {i + 1} is hidden: {isHidden}");
            }

            // احفظ المصنف
            workbook.Save("RowHiddenDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


