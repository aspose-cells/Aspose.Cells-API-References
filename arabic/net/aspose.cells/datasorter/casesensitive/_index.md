---
title: "DataSorter.CaseSensitive"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataSorter. يحصل ويضبط ما إذا كان حساسًا لحالة الأحرف عند مقارنة السلسلة"
type: docs
url: /ar/net/aspose.cells/datasorter/casesensitive/
---
## DataSorter.CaseSensitive property

يحصل ويضبط ما إذا كان حساسًا لحالة الأحرف عند مقارنة السلسلة.

```csharp
public bool CaseSensitive { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyCaseSensitiveDemo
    {
        public static void Run()
        {
            // إنشاء مصنف وورقة عمل
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // أضف بيانات عينة مع اختلافات في حالة الأحرف
            cells["A1"].PutValue("apple");
            cells["A2"].PutValue("Orange");
            cells["A3"].PutValue("banana");
            cells["A4"].PutValue("APPLE");
            cells["A5"].PutValue("orange");
            cells["A6"].PutValue("Banana");

            // إنشاء أداة فرز البيانات
            DataSorter sorter = workbook.DataSorter;
            sorter.Key1 = 0; // Sort by first column
            sorter.Order1 = SortOrder.Ascending;

            // عرض فرز حساس لحالة الأحرف
            Console.WriteLine("Sorting with CaseSensitive = true:");
            sorter.CaseSensitive = true;
            sorter.Sort(cells, CellArea.CreateCellArea("A1", "A6"));
            PrintSortedData(cells, "A1:A6");

            // عرض فرز غير حساس لحالة الأحرف
            Console.WriteLine("\nSorting with CaseSensitive = false:");
            sorter.CaseSensitive = false;
            sorter.Sort(cells, CellArea.CreateCellArea("A1", "A6"));
            PrintSortedData(cells, "A1:A6");
        }

        private static void PrintSortedData(Cells cells, string range)
        {
            Console.WriteLine("Sorted data:");
            foreach (Cell cell in cells.CreateRange(range))
            {
                Console.WriteLine(cell.StringValue);
            }
        }
    }
}
```

### انظر أيضًا

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


