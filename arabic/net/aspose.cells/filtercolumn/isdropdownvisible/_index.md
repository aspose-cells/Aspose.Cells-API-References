---
title: "FilterColumn.IsDropdownVisible"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FilterColumn. تشير إلى ما إذا كان زر AutoFilter لهذا العمود مرئيًا"
type: docs
url: /ar/net/aspose.cells/filtercolumn/isdropdownvisible/
---
## FilterColumn.IsDropdownVisible property

يشير إلى ما إذا كان زر AutoFilter لهذا العمود مرئيًا.

```csharp
public bool IsDropdownVisible { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyIsDropdownVisibleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["A4"].PutValue("Fruit");

            // تطبيق AutoFilter
            sheet.AutoFilter.SetRange(0, 0, 3);  // Fixed: Using row/column indices instead of range string

            // احصل على عمود الفلتر
            FilterColumn filterColumn = sheet.AutoFilter.FilterColumns[0];

            // إظهار القائمة المنسدلة مبدئيًا
            filterColumn.IsDropdownVisible = true;
            Console.WriteLine($"Initial IsDropdownVisible: {filterColumn.IsDropdownVisible}");

            // إخفاء القائمة المنسدلة
            filterColumn.IsDropdownVisible = false;
            Console.WriteLine($"After setting to false: {filterColumn.IsDropdownVisible}");

            // احفظ المصنف
            workbook.Save("FilterColumnDropdownDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


