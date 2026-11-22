---
title: "Cells.UnhideRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تُظهر صفًا مخفيًا"
type: docs
url: /ar/net/aspose.cells/cells/unhiderow/
---
## Cells.UnhideRow method

يكشف عن صف.

```csharp
public void UnhideRow(int row, double height)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| الارتفاع | Double | ارتفاع الصف. سيتغير ارتفاع الصف فقط عندما يكون الصف مخفيًا وتكون قيمة الارتفاع المعطاة موجبة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUnhideRowWithInt32DoubleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إخفاء الصف 5
            worksheet.Cells.HideRow(5);
            
            // إظهار الصف 5 بارتفاع 12.75
            worksheet.Cells.UnhideRow(5, 12.75);
            
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


