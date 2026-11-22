---
title: "FilterColumn.IconFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FilterColumn. يحصل على IconFilter لتصفية البيانات حسب الأيقونة"
type: docs
url: /ar/net/aspose.cells/filtercolumn/iconfilter/
---
## FilterColumn.IconFilter property

يحصل على `IconFilter` لتصفية البيانات حسب الأيقونة.

```csharp
public IconFilter IconFilter { get; }
```

### ملاحظات

قبل استخدام هذه الخاصية، يرجى التأكد من أن [`FilterType`](../filtertype/) هو IconFilter، وإلا سيتم إرجاع null.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyIconFilterDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // أضف بيانات عينة مع تنسيق شرطي يستخدم الأيقونات
                worksheet.Cells["A1"].PutValue("Performance");
                worksheet.Cells["A2"].PutValue(85);
                worksheet.Cells["A3"].PutValue(72);
                worksheet.Cells["A4"].PutValue(93);
                worksheet.Cells["A5"].PutValue(65);

                // تطبيق الفلتر التلقائي على النطاق
                worksheet.AutoFilter.Range = "A1:A5";

                // احصل على عمود الفلتر
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // الوصول إلى خاصية IconFilter (للقراءة فقط)
                IconFilter iconFilter = filterColumn.IconFilter;

                // عرض خصائص IconFilter إذا كانت موجودة
                if (iconFilter != null)
                {
                    Console.WriteLine("IconFilter is available");
                    Console.WriteLine($"IconSetType: {iconFilter.IconSetType}");
                    Console.WriteLine($"IconId: {iconFilter.IconId}");
                }
                else
                {
                    Console.WriteLine("No IconFilter is currently applied to this column");
                }

                // احفظ المصنف
                workbook.Save("IconFilterDemo.xlsx");
                Console.WriteLine("IconFilter demonstration completed successfully.");
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

* class [IconFilter](../../iconfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


