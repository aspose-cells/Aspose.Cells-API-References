---
title: "الفئة FilterColumnCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.FilterColumnCollection. مجموعة من كائنات Filter تمثل جميع الفلاتر في نطاق مُصفّى تلقائيًا"
type: docs
url: /ar/net/aspose.cells/filtercolumncollection/
---
## FilterColumnCollection class

مجموعة من كائنات Filter تمثل جميع المرشحات في نطاق مُفلتر تلقائيًا.

```csharp
public class FilterColumnCollection : CollectionBase<FilterColumn>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/filtercolumncollection/item/) { get; } | يحصل على كائن [`FilterColumn`](../filtercolumn/) في الحقل الخاص. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FilterColumn) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(FilterColumn, IComparer&lt;FilterColumn&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, FilterColumn, IComparer&lt;FilterColumn&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(FilterColumn) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FilterColumn[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(FilterColumn[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, FilterColumn[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;FilterColumn&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;FilterColumn&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;FilterColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;FilterColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;FilterColumn&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;FilterColumn&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;FilterColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;FilterColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;FilterColumn&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;FilterColumn&gt;) |  |
| [GetByIndex](../../aspose.cells/filtercolumncollection/getbyindex/)(int) | يرجع كائن Filter واحد من مجموعة. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FilterColumn) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FilterColumn, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(FilterColumn, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FilterColumn) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FilterColumn, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(FilterColumn, int, int) |  |
| [RemoveAt](../../aspose.cells/filtercolumncollection/removeat/#removeat)(int) | (طريقتان) |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnCollectionDemo
    {
        public static void FilterColumnCollectionExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات إلى الفلتر
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["A4"].PutValue("Doe");
            worksheet.Cells["B4"].PutValue(22);

            // إنشاء AutoFilter
            worksheet.AutoFilter.Range = "A1:B4";

            // احصل على FilterColumnCollection
            FilterColumnCollection filterColumns = worksheet.AutoFilter.FilterColumns;

            // إضافة مرشح إلى العمود الثاني (Age)
            worksheet.AutoFilter.AddFilter(1, "25");

            // تطبيق الفلتر
            worksheet.AutoFilter.Refresh();

            // الوصول إلى مجموعة أعمدة الفلتر والتعامل معها
            Console.WriteLine("Number of filters applied: " + filterColumns.Count);

            // الحصول على أول عمود فلتر
            FilterColumn filterColumn = filterColumns.GetByIndex(0);
            Console.WriteLine("Filter applied on column index: " + filterColumn.FieldIndex);

            // إزالة الفلتر
            filterColumns.RemoveAt(0);
            worksheet.AutoFilter.Refresh();

            // احفظ المصنف
            workbook.Save("FilterColumnCollectionExample.xlsx");
            workbook.Save("FilterColumnCollectionExample.pdf");
        }
    }
}
```

### انظر أيضًا

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [FilterColumn](../filtercolumn/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


