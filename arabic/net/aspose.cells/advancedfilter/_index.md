---
title: "الفئة AdvancedFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.AdvancedFilter. تمثل إعدادات الفلتر المتقدم"
type: docs
url: /ar/net/aspose.cells/advancedfilter/
---
## AdvancedFilter class

يمثل إعدادات الفلتر المتقدم.

```csharp
public class AdvancedFilter
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CopyToRange](../../aspose.cells/advancedfilter/copytorange/) { get; } | يحصل على النطاق الذي يتم نسخ نتيجة هذا الفلتر المتقدم إليه. |
| [CriteriaRange](../../aspose.cells/advancedfilter/criteriarange/) { get; } | يحصل على نطاق المعايير لهذا الفلتر المتقدم. |
| [ListRange](../../aspose.cells/advancedfilter/listrange/) { get; } | يحصل على نطاق القائمة لهذا الفلتر المتقدم. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassAdvancedFilterDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // املأ بيانات عينة لنطاق القائمة
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["B2"].PutValue(1.5);
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["B3"].PutValue(0.8);
                worksheet.Cells["A4"].PutValue("Orange");
                worksheet.Cells["B4"].PutValue(1.2);

                // املأ نطاق المعايير
                worksheet.Cells["D1"].PutValue("Product");
                worksheet.Cells["D2"].PutValue("Apple");

                // احصل على نسخة AdvancedFilter من ورقة العمل
                AdvancedFilter advancedFilter = worksheet.GetAdvancedFilter();

                // اعرض الخصائص للقراءة فقط
                Console.WriteLine("List Range: " + advancedFilter.ListRange);
                Console.WriteLine("Criteria Range: " + advancedFilter.CriteriaRange);
                Console.WriteLine("Copy To Range: " + advancedFilter.CopyToRange);

                // احفظ المصنف
                workbook.Save("AdvancedFilterDemo.xlsx");
                Console.WriteLine("AdvancedFilter demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in AdvancedFilter demonstration: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


