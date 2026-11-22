---
title: "FilterColumn.ColorFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FilterColumn. يحصل على ColorFilter لتصفية البيانات حسب اللون"
type: docs
url: /ar/net/aspose.cells/filtercolumn/colorfilter/
---
## FilterColumn.ColorFilter property

يحصل على [`ColorFilter`](../../colorfilter/) لتصفية البيانات حسب اللون.

```csharp
public ColorFilter ColorFilter { get; }
```

### ملاحظات

يضبط [`FilterType`](../filtertype/) كـ ColorFilter أولاً، وإلا سيتم إرجاع Null.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyColorFilterDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // إضافة بيانات عينة مع ألوان
                worksheet.Cells["A1"].PutValue("Color");
                worksheet.Cells["A2"].PutValue("Red");
                worksheet.Cells["A3"].PutValue("Blue");
                worksheet.Cells["A4"].PutValue("Green");

                // تطبيق الفلتر التلقائي
                worksheet.AutoFilter.Range = "A1:A4";

                // احصل على عمود الفلتر
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // الوصول إلى خاصية ColorFilter (للقراءة فقط)
                ColorFilter colorFilter = filterColumn.ColorFilter;

                // عرض خصائص ColorFilter
                if (colorFilter != null)
                {
                    Console.WriteLine("ColorFilter is not null");
                    Console.WriteLine("FilterByFillColor: " + colorFilter.FilterByFillColor);
                }
                else
                {
                    Console.WriteLine("ColorFilter is null (no color filter applied)");
                }

                // احفظ المصنف
                workbook.Save("ColorFilterDemo.xlsx");
                Console.WriteLine("ColorFilter demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ColorFilter](../../colorfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


