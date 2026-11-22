---
title: "Cells.HideGroupDetail"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تُطوي الصفوف/الأعمدة المجمعة"
type: docs
url: /ar/net/aspose.cells/cells/hidegroupdetail/
---
## Cells.HideGroupDetail method

يطوي الصفوف/الأعمدة المجمعة.

```csharp
public void HideGroupDetail(bool isVertical, int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| isVertical | منطقي | صحيح، اطوي الصفوف المجمعة. |
| فهرس | Int32 | مؤشر الصف/العمود |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideGroupDetailWithBooleanInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // جمّع الصفوف وأخفِ التفاصيل
            worksheet.Cells.GroupRows(0, 9, false);
            worksheet.Cells.HideGroupDetail(true, 4);
            worksheet.Cells.HideGroupDetail(true, 7);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


