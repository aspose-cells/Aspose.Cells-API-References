---
title: "Cells.GetViewRowHeight"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحصل على ارتفاع صف محدد"
type: docs
url: /ar/net/aspose.cells/cells/getviewrowheight/
---
## Cells.GetViewRowHeight method

يحصل على ارتفاع الصف المحدد.

```csharp
public double GetViewRowHeight(int row)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |

### قيمة الإرجاع

ارتفاع الصف.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetViewRowHeightWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين ارتفاع الصف للصف 3 (بالنقاط)
            worksheet.Cells.SetRowHeight(3, 15);
            
            // الحصول على ارتفاع صف العرض للصف 3
            double viewRowHeight = worksheet.Cells.GetViewRowHeight(3);
            
            // أخرج النتيجة.
            Console.WriteLine("View Row Height for row 3: " + viewRowHeight);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


