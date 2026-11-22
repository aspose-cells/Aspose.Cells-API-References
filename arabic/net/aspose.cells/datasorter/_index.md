---
title: "فئة DataSorter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.DataSorter. وصف موجز لـ DataSorter"
type: docs
url: /ar/net/aspose.cells/datasorter/
---
## DataSorter class

وصف موجز لـ DataSorter.

```csharp
public class DataSorter
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CaseSensitive](../../aspose.cells/datasorter/casesensitive/) { get; set; } | يحصل ويضبط ما إذا كان حساسًا لحالة الأحرف عند مقارنة السلسلة. |
| [HasHeaders](../../aspose.cells/datasorter/hasheaders/) { get; set; } | يمثل ما إذا كان النطاق يحتوي على رؤوس. |
| [Key1](../../aspose.cells/datasorter/key1/) { get; set; } | يمثل فهرس العمود المرتب الأول (الموضع المطلق، العمود A هو 0، B هو 1، ...). |
| [Key2](../../aspose.cells/datasorter/key2/) { get; set; } | يمثل فهرس العمود المرتب الثاني (الموضع المطلق، العمود A هو 0، B هو 1، ...). |
| [Key3](../../aspose.cells/datasorter/key3/) { get; set; } | يمثل فهرس العمود المرتب الثالث (الموضع المطلق، العمود A هو 0، B هو 1، ...). |
| [Keys](../../aspose.cells/datasorter/keys/) { get; } | يحصل على قائمة المفاتيح لفرز البيانات. |
| [Order1](../../aspose.cells/datasorter/order1/) { get; set; } | يمثل ترتيب الفرز للمفتاح الأول. |
| [Order2](../../aspose.cells/datasorter/order2/) { get; set; } | يمثل ترتيب الفرز للمفتاح الثاني. |
| [Order3](../../aspose.cells/datasorter/order3/) { get; set; } | يمثل ترتيب الفرز للمفتاح الثالث. |
| [SortAsNumber](../../aspose.cells/datasorter/sortasnumber/) { get; set; } | يشير إلى ما إذا كان يتم فرز أي شيء يبدو كرقم. |
| [SortLeftToRight](../../aspose.cells/datasorter/sortlefttoright/) { get; set; } | صحيح يعني أن اتجاه الفرز من اليسار إلى اليمين. خطأ يعني أن اتجاه الفرز من الأعلى إلى الأسفل. القيمة الافتراضية هي خطأ. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AddColorKey](../../aspose.cells/datasorter/addcolorkey/)(int, SortOnType, SortOrder, Color) | يضيف مفتاح فرز اللون. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_1)(int, SortOrder) | يضيف فهرس العمود المرتب وترتيب الفرز. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_2)(int, SortOrder, string) | يضيف فهرس العمود المرتب وترتيب الفرز مع قائمة فرز مخصصة. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey_3)(int, SortOrder, string[]) | يضيف فهرس العمود المرتب وترتيب الفرز مع قائمة فرز مخصصة. |
| [AddKey](../../aspose.cells/datasorter/addkey/#addkey)(int, SortOnType, SortOrder, object) | يضيف فهرس العمود المرتب وترتيب الفرز مع قائمة فرز مخصصة. |
| [Clear](../../aspose.cells/datasorter/clear/)() | امسح جميع الإعدادات. |
| [Sort](../../aspose.cells/datasorter/sort/#sort)() | رتّب البيانات في النطاق. |
| [Sort](../../aspose.cells/datasorter/sort/#sort_1)(Cells, CellArea) | رتّب بيانات المنطقة. |
| [Sort](../../aspose.cells/datasorter/sort/#sort_2)(Cells, int, int, int, int) | يرتب بيانات المنطقة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterDemo
    {
        public static void DataSorterExample()
        {
            // إنشاء كائن Workbook جديد
            Workbook workbook = new Workbook("DataSorter_original.xlsx");

            // احصل على كائن DataSorter للـWorkbook
            DataSorter sorter = workbook.DataSorter;

            // حدد الترتيب الأول لكائن DataSorter
            sorter.Order1 = SortOrder.Descending;
            // حدد المفتاح الأول
            sorter.Key1 = 0;

            // حدد الترتيب الثاني لكائن DataSorter
            sorter.Order2 = SortOrder.Ascending;
            // حدد المفتاح الثاني
            sorter.Key2 = 1;

            // إنشاء منطقة خلايا (نطاق)
            CellArea ca = new CellArea
            {
                StartRow = 0,
                StartColumn = 0,
                EndRow = 13,
                EndColumn = 1
            };

            // رتّب البيانات في نطاق البيانات المحدد (A1:B14)
            sorter.Sort(workbook.Worksheets[0].Cells, ca);

            // احفظ ملف Excel
            workbook.Save("DataSorterExample.xlsx");
            workbook.Save("DataSorterExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


