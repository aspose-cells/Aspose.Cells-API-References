---
title: "Class DataSorterKey"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.DataSorterKey. تمثل مفتاح مُرتّب البيانات"
type: docs
url: /ar/net/aspose.cells/datasorterkey/
---
## DataSorterKey class

يمثل المفتاح لمرتب البيانات DataSorter.

```csharp
public class DataSorterKey
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Color](../../aspose.cells/datasorterkey/color/) { get; } | يحصل على اللون المرتّب. |
| [IconId](../../aspose.cells/datasorterkey/iconid/) { get; } | يمثل المعرف لنوع مجموعة الأيقونات. |
| [IconSetType](../../aspose.cells/datasorterkey/iconsettype/) { get; } | يمثل نوع مجموعة الأيقونات. |
| [Index](../../aspose.cells/datasorterkey/index/) { get; } | يحصل على فهرس العمود المرتّب (الموضع المطلق، العمود A هو 0، B هو 1، ...) |
| [Order](../../aspose.cells/datasorterkey/order/) { get; } | يشير إلى ترتيب الفرز. |
| [Type](../../aspose.cells/datasorterkey/type/) { get; } | يمثل نوع الفرز. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataSorterKeyDemo
    {
        public static void DataSorterKeyExample()
        {
            // إنشاء كائن دفتر عمل وتحميل ملف قالب
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات النموذجية للفرز
            worksheet.Cells["A1"].PutValue("USA");
            worksheet.Cells["A2"].PutValue("China");
            worksheet.Cells["A3"].PutValue("Brazil");
            worksheet.Cells["A4"].PutValue("Russia");
            worksheet.Cells["A5"].PutValue("Canada");

            // إنشاء كائن مُرتّب البيانات
            DataSorter sorter = workbook.DataSorter;

            // إضافة مفتاح للعمود الأول (A) للفرز بترتيب تصاعدي
            sorter.AddKey(0, SortOrder.Ascending);

            // إنشاء نطاق خلايا (مجال) للفرز
            CellArea ca = CellArea.CreateCellArea("A1", "A5");

            // تنفيذ الفرز
            sorter.Sort(worksheet.Cells, ca);

            // حفظ ملف الإخراج
            workbook.Save("DataSorterKeyExample.xlsx");
            workbook.Save("DataSorterKeyExample.pdf");

            // الوصول إلى DataSorterKeyCollection
            DataSorterKeyCollection keys = sorter.Keys;

            // التكرار عبر المفاتيح وطباعة خصائصها
            foreach (DataSorterKey key in keys)
            {
                Console.WriteLine($"Order: {key.Order}");
                Console.WriteLine($"Index: {key.Index}");
                Console.WriteLine($"Type: {key.Type}");
                Console.WriteLine($"IconSetType: {key.IconSetType}");
                Console.WriteLine($"IconId: {key.IconId}");
                Console.WriteLine($"Color: {key.Color}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


