---
title: "Row.IsCollapsed"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Row. ما إذا كان الصف مطويًا"
type: docs
url: /ar/net/aspose.cells/row/iscollapsed/
---
## Row.IsCollapsed property

ما إذا كان الصف مطويًا

```csharp
public bool IsCollapsed { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsCollapsedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء وتنسيق صف
            Row row = worksheet.Cells.Rows[0];
            row.Height = 20;
            row.GroupLevel = 1;
            
            // عرض خاصية IsCollapsed
            row.IsCollapsed = true;
            Console.WriteLine("Row is collapsed: " + row.IsCollapsed);

            // توسيع الصف
            row.IsCollapsed = false;
            Console.WriteLine("Row is collapsed: " + row.IsCollapsed);

            // احفظ المصنف
            workbook.Save("RowIsCollapsedDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


