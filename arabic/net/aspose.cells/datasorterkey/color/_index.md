---
title: "DataSorterKey.Color"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataSorterKey. تحصّل على اللون المرتب"
type: docs
url: /ar/net/aspose.cells/datasorterkey/color/
---
## DataSorterKey.Color property

يحصل على اللون المرتّب.

```csharp
public Color Color { get; }
```

### ملاحظات

يعمل فقط عندما يكون [`Type`](../type/) هو CellColor أو FontColor.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataSorterKeyPropertyColorDemo
    {
        public static void Run()
        {
            // إنشاء كائن دفتر عمل
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // إنشاء مُرتّب البيانات وإضافة المفتاح
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending);

            // فرز البيانات
            CellArea ca = CellArea.CreateCellArea("A1", "A5");
            sorter.Sort(worksheet.Cells, ca);

            // إخراج خاصية اللون من المفاتيح
            foreach (DataSorterKey k in sorter.Keys)
            {
                Console.WriteLine($"Color: {k.Color}");
            }
        }
    }
}
```

### انظر أيضًا

* class [DataSorterKey](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


