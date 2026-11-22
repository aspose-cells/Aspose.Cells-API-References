---
title: "FilterColumn.FieldIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FilterColumn. يحصل على ويضبط إزاحة العمود في النطاق"
type: docs
url: /ar/net/aspose.cells/filtercolumn/fieldindex/
---
## FilterColumn.FieldIndex property

يحصل على ويضبط إزاحة العمود في النطاق.

```csharp
public int FieldIndex { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyFieldIndexDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Department");
            worksheet.Cells["B1"].PutValue("Employees");
            worksheet.Cells["A2"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(15);
            worksheet.Cells["A3"].PutValue("Marketing");
            worksheet.Cells["B3"].PutValue(8);
            worksheet.Cells["A4"].PutValue("IT");
            worksheet.Cells["B4"].PutValue(12);

            // تطبيق الفلتر التلقائي
            worksheet.AutoFilter.Range = "A1:B4";
            
            // إضافة مرشح إلى العمود الأول (القسم)
            worksheet.AutoFilter.AddFilter(0, "Sales");

            // احصل على عمود الفلتر
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            
            // إظهار خاصية FieldIndex
            Console.WriteLine("Filter is applied on column index: " + filterColumn.FieldIndex);
            
            // تحديث وحفظ
            worksheet.AutoFilter.Refresh();
            workbook.Save("FilterColumnFieldIndexDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


