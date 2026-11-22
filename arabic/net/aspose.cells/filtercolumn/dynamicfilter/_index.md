---
title: "FilterColumn.DynamicFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FilterColumn. يحصل على DynamicFilter لتصفية باستخدام معايير ديناميكية"
type: docs
url: /ar/net/aspose.cells/filtercolumn/dynamicfilter/
---
## FilterColumn.DynamicFilter property

يحصل على `DynamicFilter` لتصفية باستخدام معايير ديناميكية.

```csharp
public DynamicFilter DynamicFilter { get; }
```

### ملاحظات

قبل استخدام هذه الخاصية، يرجى التأكد من أن [`FilterType`](../filtertype/) هو DynamicFilter، وإلا سيتم إرجاع null.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyDynamicFilterDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // أضف بيانات تجريبية
                worksheet.Cells["A1"].PutValue("Date");
                worksheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-10));
                worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(-5));
                worksheet.Cells["A4"].PutValue(DateTime.Now);

                // تطبيق الفلتر التلقائي
                worksheet.AutoFilter.Range = "A1:A4";

                // احصل على عمود الفلتر
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // الوصول إلى خاصية DynamicFilter (للقراءة فقط)
                DynamicFilter dynamicFilter = filterColumn.DynamicFilter;

                // عرض خصائص DynamicFilter
                if (dynamicFilter != null)
                {
                    Console.WriteLine("DynamicFilter is not null");
                    Console.WriteLine("DynamicFilterType: " + dynamicFilter.DynamicFilterType);
                    Console.WriteLine("Value: " + dynamicFilter.Value);
                    Console.WriteLine("MaxValue: " + dynamicFilter.MaxValue);
                }
                else
                {
                    Console.WriteLine("DynamicFilter is null (no dynamic filter applied)");
                }

                // احفظ المصنف
                workbook.Save("DynamicFilterDemo.xlsx");
                Console.WriteLine("DynamicFilter demonstration completed successfully.");
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

* class [DynamicFilter](../../dynamicfilter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


