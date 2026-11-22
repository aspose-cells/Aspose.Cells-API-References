---
title: "Cells.DeleteRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحذف نطاقًا من الخلايا وتُحرك الخلايا وفقًا لخيار shift"
type: docs
url: /ar/net/aspose.cells/cells/deleterange/
---
## Cells.DeleteRange method

يحذف نطاقًا من الخلايا ويُحَرِّك الخلايا وفقًا لخيار الإزاحة.

```csharp
public void DeleteRange(int startRow, int startColumn, int endRow, int endColumn, 
    ShiftType shiftType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | فهرس الصف الابتدائي. |
| startColumn | Int32 | فهرس العمود الابتدائي. |
| endRow | Int32 | فهرس الصف النهائي. |
| endColumn | Int32 | فهرس العمود النهائي. |
| shiftType | ShiftType | خيار إزاحة الخلايا. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRangeWithInt32Int32Int32Int32ShiftTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // املأ بعض بيانات العينة
            sheet.Cells["A1"].PutValue("A1");
            sheet.Cells["B1"].PutValue("B1");
            sheet.Cells["C1"].PutValue("C1");
            sheet.Cells["A2"].PutValue("A2");
            sheet.Cells["B2"].PutValue("B2");
            sheet.Cells["C2"].PutValue("C2");

            // احذف النطاق وحركه إلى اليسار
            sheet.Cells.DeleteRange(0, 1, 1, 2, ShiftType.Left);

            // احفظ المصنف
            workbook.Save("DeleteRangeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


