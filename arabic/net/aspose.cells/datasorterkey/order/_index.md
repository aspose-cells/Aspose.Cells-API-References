---
title: "DataSorterKey.Order"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataSorterKey. تشير إلى ترتيب الفرز"
type: docs
url: /ar/net/aspose.cells/datasorterkey/order/
---
## DataSorterKey.Order property

يشير إلى ترتيب الفرز.

```csharp
public SortOrder Order { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyOrderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // بيانات عينة
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["A4"].PutValue("Doe");
            worksheet.Cells["B4"].PutValue(80);

            DataSorter sorter = workbook.DataSorter;
            sorter.Order1 = SortOrder.Descending;
            sorter.Key1 = 1; // Sort by Score column

            CellArea area = new CellArea
            {
                StartRow = 1,
                StartColumn = 0,
                EndRow = 3,
                EndColumn = 1
            };

            sorter.Sort(worksheet.Cells, area);

            // عرض كيفية استخدام خاصية Order
            DataSorterKey key = sorter.Keys[0];
            Console.WriteLine("Key Order: " + key.Order);

            workbook.Save("DataSorterKeyOrderDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [SortOrder](../../sortorder/)
* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


