---
title: "Cells.HideColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تخفي عمودًا"
type: docs
url: /ar/net/aspose.cells/cells/hidecolumn/
---
## Cells.HideColumn method

يخفي عمودًا.

```csharp
public void HideColumn(int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | Int32 | فهرس العمود. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideColumnWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // عيّن بعض البيانات في العمود الذي سنخفيه
            cells["B1"].PutValue("This column will be hidden");
            cells["B2"].PutValue(123.45);

            // أخفِ العمود B (الفهرس 1)
            cells.HideColumn(1);

            // إظهار العمود بالعرض القياسي
            cells.UnhideColumn(1, cells.StandardWidth);

            // احفظ المصنف
            workbook.Save("HideColumnDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


