---
title: "الفئة FilterColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.FilterColumn. تمثل مرشحًا لعمود واحد أو عمود في الجدول"
type: docs
url: /ar/net/aspose.cells/filtercolumn/
---
## FilterColumn class

يمثل مرشحًا لعمود واحد أو عمود في الجدول.

```csharp
public class FilterColumn
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ColorFilter](../../aspose.cells/filtercolumn/colorfilter/) { get; } | يحصل على [`ColorFilter`](../colorfilter/) لتصفية البيانات حسب اللون. |
| [CustomFilters](../../aspose.cells/filtercolumn/customfilters/) { get; set; } | يحصل على [`CustomFilterCollection`](../customfiltercollection/) لتصفية البيانات وفقًا لمعايير مخصصة. |
| [DynamicFilter](../../aspose.cells/filtercolumn/dynamicfilter/) { get; } | يحصل على [`DynamicFilter`](./dynamicfilter/) لتصفية البيانات بمعايير ديناميكية. |
| [FieldIndex](../../aspose.cells/filtercolumn/fieldindex/) { get; set; } | يحصل على ويضبط إزاحة العمود في النطاق. |
| [Filter](../../aspose.cells/filtercolumn/filter/) { get; set; } | (**Obsolete.**) يحصل على ويضبط شرط تصفية البيانات. |
| [FilterType](../../aspose.cells/filtercolumn/filtertype/) { get; set; } | يحصل على ويضبط نوع تصفية البيانات. |
| [FilterValues](../../aspose.cells/filtercolumn/filtervalues/) { get; } | يحصل على [`FilterValueCollection`](../filtervaluecollection/) لتصفية البيانات حسب العلامات أو التاريخ والوقت. |
| [IconFilter](../../aspose.cells/filtercolumn/iconfilter/) { get; } | يحصل على [`IconFilter`](./iconfilter/) لتصفية البيانات حسب الأيقونة. |
| [IsDropdownVisible](../../aspose.cells/filtercolumn/isdropdownvisible/) { get; set; } | يشير إلى ما إذا كان زر AutoFilter لهذا العمود مرئيًا. |
| [MultipleFilters](../../aspose.cells/filtercolumn/multiplefilters/) { get; set; } | (**Obsolete.**) يحصل على [`MultipleFilterCollection`](../multiplefiltercollection/) لتصفية البيانات حسب العلامات أو التاريخ والوقت. |
| [Top10Filter](../../aspose.cells/filtercolumn/top10filter/) { get; } | يحصل على [`Top10Filter`](./top10filter/) لتصفية البيانات حسب ترتيب البيانات. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SelectAll](../../aspose.cells/filtercolumn/selectall/)() | حدد الكل. |

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;

namespace AsposeCellsExamples
{
    public class FilterColumnDemo
    {
        public static void RunDemo()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Jane");
            sheet.Cells["A4"].PutValue("Doe");

            sheet.Cells["B1"].PutValue("Age");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["B3"].PutValue(25);
            sheet.Cells["B4"].PutValue(35);

            // تطبيق AutoFilter على النطاق
            sheet.AutoFilter.SetRange(0, 0, 3);

            // إضافة مرشح إلى العمود الأول (Name)
            sheet.AutoFilter.AddFilter(0, "John");

            // إضافة مرشح إلى العمود الثاني (Age)
            sheet.AutoFilter.AddFilter(1, "30");

            // تحديث المرشح لتطبيقه
            sheet.AutoFilter.Refresh();

            // الوصول إلى FilterColumnCollection
            FilterColumnCollection filterColumns = sheet.AutoFilter.FilterColumns;

            // الوصول إلى FilterColumn الأول
            FilterColumn filterColumn = filterColumns[0];

            // عرض خصائص FilterColumn
            Console.WriteLine($"IsDropdownVisible: {filterColumn.IsDropdownVisible}");
            Console.WriteLine($"Filter: {filterColumn.Filter}");
            Console.WriteLine($"FilterType: {filterColumn.FilterType}");
            Console.WriteLine($"FieldIndex: {filterColumn.FieldIndex}");

            // احفظ المصنف
            workbook.Save("FilterColumnDemo.xlsx");
            workbook.Save("FilterColumnDemo.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


