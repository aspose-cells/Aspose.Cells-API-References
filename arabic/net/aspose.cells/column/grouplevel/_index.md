---
title: "Column.GroupLevel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Column. تحصل على مستوى التجميع للعمود"
type: docs
url: /ar/net/aspose.cells/column/grouplevel/
---
## Column.GroupLevel property

يحصل على مستوى المجموعة للعمود.

```csharp
public byte GroupLevel { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyGroupLevelDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تجميع الأعمدة (معامل isHidden مضبوط على false)
            worksheet.Cells.GroupColumns(0, 2, false);
            
            // احصل على مستوى التجميع للعمود الأول
            int groupLevel = worksheet.Cells.Columns[0].GroupLevel;
            
            // إخراج مستوى التجميع
            Console.WriteLine("Group level of first column: " + groupLevel);
            
            // احفظ المصنف
            workbook.Save("GroupLevelDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


