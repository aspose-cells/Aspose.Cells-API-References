---
title: "FilterColumn.MultipleFilters"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FilterColumn. يحصل على MultipleFilterCollection لتصفية البيانات حسب التسميات أو التاريخ والوقت"
type: docs
url: /ar/net/aspose.cells/filtercolumn/multiplefilters/
---
## FilterColumn.MultipleFilters property

يحصل على [`MultipleFilterCollection`](../../multiplefiltercollection/) لتصفية البيانات حسب التسميات أو التاريخ والوقت.

```csharp
[Obsolete("Use FilterColumn.FilterValues instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MultipleFilterCollection MultipleFilters { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام خاصية FilterColumn.FilterValues. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FilterColumnPropertyMultipleFiltersDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // أضف بيانات تجريبية
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("Fruit");
                worksheet.Cells["A3"].PutValue("Vegetable");
                worksheet.Cells["A4"].PutValue("Fruit");
                worksheet.Cells["A5"].PutValue("Grain");

                // تطبيق AutoFilter على النطاق
                worksheet.AutoFilter.Range = "A1:A5";

                // الحصول على أول عمود فلتر
                FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];

                // إنشاء وتعيين MultipleFilters
                MultipleFilterCollection multipleFilters = new MultipleFilterCollection();
                multipleFilters.Add("Fruit");
                multipleFilters.Add("Vegetable");
                multipleFilters.MatchBlank = false;

                // تعيين MultipleFilters إلى عمود الفلتر
                filterColumn.MultipleFilters = multipleFilters;

                // عرض خصائص MultipleFilters
                Console.WriteLine("MultipleFilters Count: " + filterColumn.MultipleFilters.Count);
                Console.WriteLine("MatchBlank: " + filterColumn.MultipleFilters.MatchBlank);

                // احفظ المصنف
                workbook.Save("MultipleFiltersDemo.xlsx");
                Console.WriteLine("MultipleFilters demonstration completed successfully.");
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

* class [MultipleFilterCollection](../../multiplefiltercollection/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


