---
title: "UnionRange.CellCount"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية UnionRange. يحصل على إجمالي عدد الخلايا في النطاق"
type: docs
url: /ar/net/aspose.cells/unionrange/cellcount/
---
## UnionRange.CellCount property

يحصل على عدد جميع الخلايا في النطاق.

```csharp
public int CellCount { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyCellCountDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء البيانات في ورقة العمل
            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].Value = $"Cell {row + 1},{col + 1}";
                }
            }

            // إنشاء نطاقات ودمجها في نطاق اتحاد
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B3");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("D1:E4");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // عرض خاصية CellCount
            Console.WriteLine("Total cells in union range: " + unionRange.CellCount);

            // حساب عدد الخلايا المتوقع
            int expectedCount = (range1.RowCount * range1.ColumnCount) + (range2.RowCount * range2.ColumnCount);
            Console.WriteLine("Expected cell count: " + expectedCount);

            // إظهار الاستخدام عن طريق التكرار عبر الخلايا
            Console.WriteLine("\nCell values in the union range:");
            int cellCounter = 0;
            foreach (Cell cell in unionRange)
            {
                Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                cellCounter++;
            }

            // تحقق من أن عدد الخلايا يطابق التكرار
            Console.WriteLine($"\nIterated through {cellCounter} cells (should match CellCount)");

            // إنشاء نطاق اتحاد آخر بأبعاد مختلفة
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("A5:E5");
            Aspose.Cells.Range range4 = worksheet.Cells.CreateRange("C1:C5");
            UnionRange unionRange2 = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range3, range4 });

            // قارن عدد الخلايا في نطاقات الاتحاد المختلفة
            Console.WriteLine("\nSecond union range cell count: " + unionRange2.CellCount);
            Console.WriteLine("First union range has " + 
                (unionRange.CellCount > unionRange2.CellCount ? "more" : "fewer") + 
                " cells than second union range");

            // احفظ المصنف
            workbook.Save("UnionRangeCellCountDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


