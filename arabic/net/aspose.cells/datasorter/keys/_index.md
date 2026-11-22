---
title: "DataSorter.Keys"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataSorter. تحصل على قائمة المفاتيح لفرّاز البيانات"
type: docs
url: /ar/net/aspose.cells/datasorter/keys/
---
## DataSorter.Keys property

يحصل على قائمة المفاتيح لفرز البيانات.

```csharp
public DataSorterKeyCollection Keys { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterPropertyKeysDemo
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

            // تهيئة فرّاز البيانات
            DataSorter sorter = workbook.DataSorter;
            
            // إضافة مفتاح فرز للعمود A (الفهرس 0)
            sorter.AddKey(0, SortOrder.Ascending);

            // فرز البيانات
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A5"));

            // عرض استخدام خاصية Keys
            DataSorterKeyCollection keys = sorter.Keys;
            Console.WriteLine("Sort Keys Information:");
            foreach (DataSorterKey key in keys)
            {
                Console.WriteLine($"Column Index: {key.Index}, Sort Order: {key.Order}");
            }

            // احفظ المصنف
            workbook.Save("DataSorterKeysDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DataSorterKeyCollection](../../datasorterkeycollection/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


