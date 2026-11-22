---
title: "Worksheet.FirstVisibleRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تمثل فهرس الصف الأول الظاهر"
type: docs
url: /ar/net/aspose.cells/worksheet/firstvisiblerow/
---
## Worksheet.FirstVisibleRow property

يمثل فهرس الصف الأول الظاهر.

```csharp
public int FirstVisibleRow { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyFirstVisibleRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // قم بتعيين بعض البيانات النموذجية
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }
            
            // تعيين الصف الأول الظاهر إلى الصف 20
            worksheet.FirstVisibleRow = 20;
            
            // عرض الصف الأول الظاهر
            Console.WriteLine("First visible row: " + worksheet.FirstVisibleRow);
            
            // احفظ المصنف
            workbook.Save("FirstVisibleRowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


