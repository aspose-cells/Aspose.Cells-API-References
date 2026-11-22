---
title: "Cells.AddRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تُضيف مرجع كائن نطاق إلى الخلايا"
type: docs
url: /ar/net/aspose.cells/cells/addrange/
---
## Cells.AddRange method

يضيف مرجع كائن نطاق إلى الخلايا

```csharp
public void AddRange(Range rangeObject)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rangeObject | النطاق | سيتم احتواء كائن النطاق في الخلايا |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodAddRangeWithRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // حدد بعض البيانات النموذجية في النطاق
            cells["A1"].PutValue("A1");
            cells["A2"].PutValue("A2");
            cells["B1"].PutValue("B1");
            cells["B2"].PutValue("B2");

            // أنشئ نطاقًا وأضفه باستخدام AddRange
            Aspose.Cells.Range range = cells.CreateRange("A1", "B2");
            cells.AddRange(range);

            // عدّل ورقة العمل لتوضيح توسيع النطاق
            cells.InsertRow(1);
            cells.InsertColumn(1);

            Console.WriteLine($"Range now has {range.RowCount} rows and {range.ColumnCount} columns");
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


