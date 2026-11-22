---
title: "Worksheet.FirstVisibleColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تمثل فهرس العمود الأول الظاهر"
type: docs
url: /ar/net/aspose.cells/worksheet/firstvisiblecolumn/
---
## Worksheet.FirstVisibleColumn property

يمثل فهرس العمود الأول الظاهر.

```csharp
public int FirstVisibleColumn { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyFirstVisibleColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إخفاء العمود الأول (الفهرس 0)
            worksheet.Cells.HideColumn(0);
            
            // احصل على وعرض فهرس العمود الأول الظاهر
            Console.WriteLine("First visible column index: " + worksheet.FirstVisibleColumn);
            
            // احفظ المصنف
            workbook.Save("FirstVisibleColumnDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


