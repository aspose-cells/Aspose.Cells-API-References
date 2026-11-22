---
title: "Cells.MoveRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحرك النطاق"
type: docs
url: /ar/net/aspose.cells/cells/moverange/
---
## Cells.MoveRange method

ينقل النطاق.

```csharp
public void MoveRange(CellArea sourceArea, int destRow, int destColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceArea | CellArea | النطاق الذي يجب تحريكه. |
| destRow | Int32 | صف الوجهة. |
| destColumn | Int32 | عمود الوجهة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMoveRangeWithCellAreaInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // ضع القيم في الخلايا
            cells["A1"].PutValue("Original");
            cells["B1"].PutValue(100);
            cells["A2"].PutValue("Data");
            cells["B2"].PutValue(200);

            // حدد نطاق الخلايا للتحريك (A1:B2)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 1;
            area.EndColumn = 1;

            // حرك النطاق إلى الأسفل بمقدار صفين وإلى اليمين بمقدار 3 أعمدة
            cells.MoveRange(area, 2, 3);

            // احفظ المصنف
            workbook.Save("MoveRangeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


