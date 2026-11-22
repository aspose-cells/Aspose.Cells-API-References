---
title: "FilterColumn.FilterType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FilterColumn. يحصل ويضبط نوع بيانات التصفية"
type: docs
url: /ar/net/aspose.cells/filtercolumn/filtertype/
---
## FilterColumn.FilterType property

يحصل على ويضبط نوع تصفية البيانات.

```csharp
public FilterType FilterType { get; set; }
```

### ملاحظات

سيتم إنشاء كائن الفلتر المقابل عندما يتم تعيين هذه الخاصية ويجب استخدام الخاصية المقابلة للحصول على كائن الفلتر وفقًا لذلك:

| **FilterType** | **Property** |
| --- | --- |
| MultipleFilters | [`FilterValues`](../filtervalues/) |
| CustomFilters | [`CustomFilters`](../customfilters/) |
| ColorFilter | [`ColorFilter`](../colorfilter/) |
| DynamicFilter | [`DynamicFilter`](../dynamicfilter/) |
| IconFilter | [`IconFilter`](../iconfilter/) |
| Top10 | [`Top10Filter`](../top10filter/) |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFilterTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Department");
            sheet.Cells["A2"].PutValue("HR");
            sheet.Cells["A3"].PutValue("IT");
            sheet.Cells["A4"].PutValue("Finance");

            sheet.Cells["B1"].PutValue("Employees");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(15);
            sheet.Cells["B4"].PutValue(8);

            // تطبيق الفلتر التلقائي باستخدام نطاق النص
            sheet.AutoFilter.Range = "A1:B4";

            // إضافة أنواع مختلفة من الفلاتر لإظهار خاصية FilterType
            sheet.AutoFilter.AddFilter(0, "HR"); // Simple filter
            sheet.AutoFilter.Custom(1, FilterOperatorType.GreaterThan, 10); // Custom filter

            // الحصول على أعمدة الفلتر
            FilterColumnCollection filterColumns = sheet.AutoFilter.FilterColumns;

            // عرض FilterType لكل عمود
            for (int i = 0; i < filterColumns.Count; i++)
            {
                FilterColumn filterColumn = filterColumns[i];
                Console.WriteLine($"Column {i} FilterType: {filterColumn.FilterType}");
            }

            // احفظ المصنف
            workbook.Save("FilterTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [FilterType](../../filtertype/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


