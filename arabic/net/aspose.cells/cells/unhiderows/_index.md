---
title: "Cells.UnhideRows"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تُظهر الصفوف المخفية"
type: docs
url: /ar/net/aspose.cells/cells/unhiderows/
---
## Cells.UnhideRows method

يكشف عن الصفوف المخفية.

```csharp
public void UnhideRows(int row, int totalRows, double height)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| totalRows | Int32 | رقم الصف. |
| الارتفاع | Double | ارتفاع الصف. سيتغير ارتفاع الصف فقط عندما يكون الصف مخفيًا وتكون قيمة الارتفاع المعطاة موجبة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideRowsWithInt32Int32DoubleDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // إخفاء الصفوف 0-4
            cells.HideRows(0, 5);
            
            // إظهار الصفوف 0-4 مع تعديل الارتفاع (-1 للتناسب التلقائي)
            cells.UnhideRows(0, 5, -1);
            
            // تحقق من أن الصفوف تم إظهارها
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine($"Row {i} hidden status: {cells.IsRowHidden(i)}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


