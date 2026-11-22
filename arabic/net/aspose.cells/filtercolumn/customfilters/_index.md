---
title: "FilterColumn.CustomFilters"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FilterColumn. يحصل على CustomFilterCollection لتصفية البيانات وفقًا لمعايير مخصصة"
type: docs
url: /ar/net/aspose.cells/filtercolumn/customfilters/
---
## FilterColumn.CustomFilters property

يحصل على [`CustomFilterCollection`](../../customfiltercollection/) لتصفية البيانات وفقًا لمعايير مخصصة.

```csharp
public CustomFilterCollection CustomFilters { get; set; }
```

### ملاحظات

ملاحظة: تم إهمال setter لهذه الخاصية الآن. بدلاً من ذلك، يرجى استخدام الخاصية [`FilterType`](../filtertype/) عن طريق تعيينها كـ CustomFilters. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyCustomFiltersDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // أضف بيانات تجريبية
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["A4"].PutValue("Cherry");
                worksheet.Cells["A5"].PutValue("Date");
                worksheet.Cells["A6"].PutValue("Elderberry");

                // تطبيق الفلتر التلقائي
                worksheet.AutoFilter.Range = "A1:A6";

                // احصل على عمود الفلتر
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // أنشئ واضبط الفلاتر المخصصة باستخدام طريقة AutoFilter.Custom
                // الفلتر الأول: يبدأ بـ "A"
                worksheet.AutoFilter.Custom(0, FilterOperatorType.BeginsWith, "A", false, FilterOperatorType.None, null);

                // الفلتر الثاني: ينتهي بـ "y" (علاقة AND)
                worksheet.AutoFilter.Custom(0, FilterOperatorType.EndsWith, "y", true, FilterOperatorType.None, null);

                // احصل على الفلاتر المخصصة من عمود الفلتر
                CustomFilterCollection customFilters = filterColumn.CustomFilters;

                // اعرض معلومات الفلاتر المخصصة
                Console.WriteLine($"Number of custom filters: {customFilters.Count}");
                Console.WriteLine($"Filter relationship (And): {customFilters.And}");

                // ملاحظة: لا تعرض CustomFilterCollection الفلاتر الفردية مباشرة
                // من خلال الفهرس، لذا لا يمكننا إلا عرض خصائص المجموعة
                Console.WriteLine("Custom filters have been applied to the column.");

                // احفظ المصنف
                workbook.Save("CustomFiltersDemo.xlsx");
                Console.WriteLine("CustomFilters demonstration completed successfully.");
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

* class [CustomFilterCollection](../../customfiltercollection/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


