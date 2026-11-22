---
title: "Row.GroupLevel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Row. تحصل على مستوى التجميع للصف"
type: docs
url: /ar/net/aspose.cells/row/grouplevel/
---
## Row.GroupLevel property

يحصل على مستوى المجموعة للصف.

```csharp
public byte GroupLevel { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyGroupLevelDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تجميع الصفوف 4-6 (مخفي = false)
            worksheet.Cells.GroupRows(3, 5, false);

            // الوصول إلى مستوى التجميع للصف 4
            int groupLevel = worksheet.Cells.Rows[3].GroupLevel;
            Console.WriteLine("Group level of row 4: " + groupLevel);

            // إلغاء تجميع الصفوف
            worksheet.Cells.UngroupRows(3, 5);
        }
    }
}
```

### انظر أيضًا

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


