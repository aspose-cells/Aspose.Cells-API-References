---
title: "Row.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Row. تحصل على الخلية"
type: docs
url: /ar/net/aspose.cells/row/item/
---
## Row indexer

يسترجع الخلية.

```csharp
public Cell this[int column] { get; }
```

| معامل | الوصف |
| --- | --- |
| عمود | فهرس العمود |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // الوصول إلى الصف الأول
            Row row = sheet.Cells.Rows[0];
            
            // تعيين محتوى HTML بأنماط ألوان مختلفة
            row[0].HtmlString = @"<span style=""color:#ffAb68;"">TEST</span>";
            row[1].HtmlString = @"<span style=""color:inherit;"">TEST</span>";
            
            // عرض استخدام خاصية Item وإخراج الألوان
            Console.WriteLine("Cell 0 Font Color: " + row[0].GetStyle().Font.Color.Name);
            Console.WriteLine("Cell 1 Font Color: " + row[1].GetStyle().Font.Color.Name);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


