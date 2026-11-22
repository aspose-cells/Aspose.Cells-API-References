---
title: "Worksheet.MoveTo"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Worksheet method. ينقل الورقة إلى موقع آخر في جدول البيانات"
type: docs
url: /ar/net/aspose.cells/worksheet/moveto/
---
## Worksheet.MoveTo method

ينقل الورقة إلى موقع آخر في جدول البيانات.

```csharp
public void MoveTo(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | فهرس الورقة الهدف. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodMoveToWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف بعض أوراق العمل
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // أضف ورقة عمل جديدة وانقلها إلى الموضع 1
            Worksheet newWorksheet = workbook.Worksheets.Add("MovedSheet");
            newWorksheet.MoveTo(1);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


