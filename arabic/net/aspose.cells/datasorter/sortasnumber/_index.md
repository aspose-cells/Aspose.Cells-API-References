---
title: "DataSorter.SortAsNumber"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataSorter. تشير إلى ما إذا كان يتم فرز أي شيء يبدو كرقم"
type: docs
url: /ar/net/aspose.cells/datasorter/sortasnumber/
---
## DataSorter.SortAsNumber property

يشير إلى ما إذا كان يتم فرز أي شيء يبدو كرقم.

```csharp
public bool SortAsNumber { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertySortAsNumberDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات عينة بأرقام مختلطة وأرقام نصية
            worksheet.Cells["A1"].PutValue("Number");
            worksheet.Cells["A2"].PutValue("2");
            worksheet.Cells["A3"].PutValue("10");
            worksheet.Cells["A4"].PutValue("1");

            // إنشاء نطاق خلايا للفرز
            CellArea ca = CellArea.CreateCellArea("A1", "A4");

            // إنشاء أداة فرز البيانات
            DataSorter sorter = workbook.DataSorter;
            int idx = CellsHelper.ColumnNameToIndex("A");

            // أضف مفتاح فرز (العمود A)
            sorter.AddKey(idx, SortOrder.Ascending);

            // فرز كأرقام (true) أو كسلاسل (false)
            sorter.SortAsNumber = true;
            sorter.Sort(worksheet.Cells, ca);

            Console.WriteLine("Sorted as numbers:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }

            // إعادة تعيين البيانات للفرز الثاني
            worksheet.Cells["A2"].PutValue("2");
            worksheet.Cells["A3"].PutValue("10");
            worksheet.Cells["A4"].PutValue("1");

            // فرز كسلاسل
            sorter.SortAsNumber = false;
            sorter.Sort(worksheet.Cells, ca);

            Console.WriteLine("\nSorted as strings:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + i].StringValue);
            }
        }
    }
}
```

### انظر أيضًا

* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


