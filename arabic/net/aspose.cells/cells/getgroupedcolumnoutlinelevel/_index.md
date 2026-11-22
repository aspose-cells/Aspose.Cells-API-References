---
title: "Cells.GetGroupedColumnOutlineLevel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحصل على مستوى المخطط للعمود (مؤشر صفر)"
type: docs
url: /ar/net/aspose.cells/cells/getgroupedcolumnoutlinelevel/
---
## Cells.GetGroupedColumnOutlineLevel method

يحصل على مستوى المخطط (بدءًا من الصفر) للعمود.

```csharp
public int GetGroupedColumnOutlineLevel(int columnIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | Int32 | فهرس العمود |

### قيمة الإرجاع

مستوى المخطط للعمود

### ملاحظات

إذا لم يتم تجميع العمود، تُعيد الصفر.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetGroupedColumnOutlineLevelWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تجميع الأعمدة (الأعمدة الثلاثة الأولى) دون إخفائها
            worksheet.Cells.GroupColumns(0, 2, false);
            
            // احصل على مستوى المخطط للعمود الأول
            int outlineLevel = worksheet.Cells.GetGroupedColumnOutlineLevel(0);
            
            Console.WriteLine("Outline level of column 0: " + outlineLevel);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


