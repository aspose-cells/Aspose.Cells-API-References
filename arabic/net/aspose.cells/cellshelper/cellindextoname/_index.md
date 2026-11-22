---
title: "CellsHelper.CellIndexToName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellsHelper. يحصل على اسم الخلية وفقًا لصفها وعمودها"
type: docs
url: /ar/net/aspose.cells/cellshelper/cellindextoname/
---
## CellsHelper.CellIndexToName method

يحصل على اسم الخلية وفقًا لمؤشرات الصف والعمود.

```csharp
public static string CellIndexToName(int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| عمود | Int32 | فهرس العمود. |

### قيمة الإرجاع

اسم الخلية.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodCellIndexToNameWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بعض البيانات
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(20);

            // احصل على اسم الخلية من مؤشرات الصف والعمود
            string cellName = CellsHelper.CellIndexToName(2, 1); // Row 2, Column 1 (B3)

            // أخرج النتيجة.
            Console.WriteLine("Cell name for row 2, column 1 is: " + cellName);
        }
    }
}
```

### انظر أيضًا

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


