---
title: "FilterColumnCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FilterColumnCollection. يحصل على كائن FilterColumn في الحقل الخاص."
type: docs
url: /ar/net/aspose.cells/filtercolumncollection/item/
---
## FilterColumnCollection indexer

يحصل على كائن [`FilterColumn`](../../filtercolumn/) في الحقل الخاص.

```csharp
public FilterColumn this[int fieldIndex] { get; }
```

| معامل | الوصف |
| --- | --- |
| fieldIndex | الإزاحة الصحيحة للحقول التي تريد بناء الفلتر عليها (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |

### قيمة الإرجاع

يرجع كائن [`FilterColumn`](../../filtercolumn/).

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Header");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");
            sheet.Cells["A5"].PutValue("Date");

            // تطبيق الفلتر التلقائي
            sheet.AutoFilter.Range = "A1:A5";
            sheet.AutoFilter.Custom(0, FilterOperatorType.Contains, "e");

            // الوصول إلى الفلتر باستخدام خاصية Item
            AutoFilter filter = sheet.AutoFilter;
            FilterColumn filterColumn = filter.FilterColumns[0]; // Using Item property
            CustomFilterCollection customFilters = (CustomFilterCollection)filterColumn.Filter;
            CustomFilter firstFilter = customFilters[0];

            // عرض خصائص الفلتر
            Console.WriteLine("Filter Operator Type: " + firstFilter.FilterOperatorType);
            Console.WriteLine("Filter Criteria: " + firstFilter.Criteria);

            // تعديل الفلتر
            firstFilter.FilterOperatorType = FilterOperatorType.EndsWith;
            Console.WriteLine("\nModified Filter Operator Type: " + firstFilter.FilterOperatorType);

            // احفظ المصنف
            wb.Save("FilterExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [FilterColumn](../../filtercolumn/)
* class [FilterColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


