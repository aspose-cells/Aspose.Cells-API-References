---
title: "Cells.GetGroupedRowOutlineLevel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحصل على مستوى المخطط الصفري للصف"
type: docs
url: /ar/net/aspose.cells/cells/getgroupedrowoutlinelevel/
---
## Cells.GetGroupedRowOutlineLevel method

يحصل على مستوى المخطط (بدءًا من الصفر) للصف.

```csharp
public int GetGroupedRowOutlineLevel(int rowIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | Int32 | فهرس الصف. |

### قيمة الإرجاع

مستوى المخطط (مبني على الصفر) للصف.

### ملاحظات

إذا لم يكن الصف مُجمّعًا، تُرجع الصفر.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetGroupedRowOutlineLevelWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تجميع الصفوف 0-3 (المستوى 1)
            cells.GroupRows(0, 3, false);
            
            // تجميع الصفوف 0-1 (المستوى 2)
            cells.GroupRows(0, 1, false);

            // احصل على مستوى المخطط لكل صف
            for (int row = 0; row <= 4; row++)
            {
                int outlineLevel = cells.GetGroupedRowOutlineLevel(row);
                Console.WriteLine($"Row {row} outline level: {outlineLevel}");
            }

            // إلغاء تجميع جميع الصفوف
            cells.UngroupRows(0, 3);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


