---
title: "Range.RowCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Range. يحصل على عدد الصفوف في النطاق"
type: docs
url: /ar/net/aspose.cells/range/rowcount/
---
## Range.RowCount property

يحصل على عدد الصفوف في النطاق.

```csharp
public int RowCount { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRowCountDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أنشئ بيانات عينة في الخلايا A1:B10
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 2; col++)
                {
                    worksheet.Cells[row, col].Value = $"Row{row + 1}Col{col + 1}";
                }
            }

            // أنشئ نطاقًا مسمى يغطي A1:B10
            worksheet.Cells.CreateRange("A1", "B10").Name = "testRange";
            
            // احصل على النطاق المسمى
            Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("testRange");
            
            // عرض خاصية RowCount
            Console.WriteLine($"Range starts at row: {range.FirstRow}");
            Console.WriteLine($"Range row count: {range.RowCount}");
            Console.WriteLine($"Range starts at column: {range.FirstColumn}");
            Console.WriteLine($"Range column count: {range.ColumnCount}");
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


