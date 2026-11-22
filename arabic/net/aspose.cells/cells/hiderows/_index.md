---
title: "Cells.HideRows"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تخفي عدة صفوف"
type: docs
url: /ar/net/aspose.cells/cells/hiderows/
---
## Cells.HideRows method

يخفي صفوفًا متعددة.

```csharp
public void HideRows(int row, int totalRows)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| totalRows | Int32 | رقم الصف. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بعض البيانات
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].Value = $"Row {i+1}, Col {j+1}";
                }
            }

            // إخفاء الصفوف 3 إلى 5 (فهرس صفرية: 2 إلى 4)
            worksheet.Cells.HideRows(2, 3);

            // احفظ المصنف
            workbook.Save("HideRowsExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


