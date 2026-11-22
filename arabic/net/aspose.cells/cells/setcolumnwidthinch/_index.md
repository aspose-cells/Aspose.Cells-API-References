---
title: "Cells.SetColumnWidthInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تُحدد عرض العمود بوحدة البوصة في العرض العادي"
type: docs
url: /ar/net/aspose.cells/cells/setcolumnwidthinch/
---
## Cells.SetColumnWidthInch method

يضبط عرض العمود بوحدة البوصة في العرض العادي.

```csharp
public void SetColumnWidthInch(int column, double inches)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | Int32 | فهرس العمود. |
| بوصات | Double | عدد البوصات. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthInchWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // حدد عرض الأعمدة بالبوصة
            cells.SetColumnWidthInch(0, 2.0);
            cells.SetColumnWidthInch(1, 1.5);
            cells.SetColumnWidthInch(2, 0.8);

            // حدد بعض البيانات في الخلايا لجعل الملف مرئيًا
            cells["A1"].PutValue("Column A (2 inches)");
            cells["B1"].PutValue("Column B (1.5 inches)");
            cells["C1"].PutValue("Column C (0.8 inches)");

            // احفظ المصنف
            workbook.Save("ColumnWidthsInInches.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


