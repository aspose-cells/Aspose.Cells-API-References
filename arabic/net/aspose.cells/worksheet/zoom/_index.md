---
title: "Worksheet.Zoom"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تمثل عامل التحجيم بالنسبة المئوية. يجب أن يكون بين 10 و400."
type: docs
url: /ar/net/aspose.cells/worksheet/zoom/
---
## Worksheet.Zoom property

يمثل عامل التحجيم بالنسبة المئوية. يجب أن يكون بين 10 و 400.

```csharp
public int Zoom { get; set; }
```

### ملاحظات

يرجى تعيين نوع العرض أولاً.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyZoomDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين عامل التكبير إلى 120%
            worksheet.Zoom = 120;
            
            // عرض عامل التكبير الحالي
            Console.WriteLine("Current worksheet zoom: " + worksheet.Zoom + "%");
            
            // احفظ المصنف
            workbook.Save("WorksheetZoomDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


