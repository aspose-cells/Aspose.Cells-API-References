---
title: "DataSorterKey.Index"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataSorterKey. تحصّل على فهرس العمود المرتب (الموقع المطلق) العمود A هو 0 والعمود B هو 1"
type: docs
url: /ar/net/aspose.cells/datasorterkey/index/
---
## DataSorterKey.Index property

يحصل على فهرس العمود المرتّب (الموضع المطلق، العمود A هو 0، B هو 1، ...)

```csharp
public int Index { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyIndexDemo
    {
        public static void Run()
        {
            // إنشاء كائن دفتر عمل
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للفرز
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // إنشاء مُرتّب البيانات وإضافة مفتاح الفرز
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // فرز البيانات
            CellArea ca = CellArea.CreateCellArea("A1", "A5");
            sorter.Sort(worksheet.Cells, ca);

            // عرض كيفية استخدام خاصية Index
            foreach (DataSorterKey key in sorter.Keys)
            {
                Console.WriteLine($"Column index being sorted: {key.Index}");
            }

            // حفظ النتيجة
            workbook.Save("DataSorterKeyExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


