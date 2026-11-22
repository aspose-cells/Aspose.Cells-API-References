---
title: "AdvancedFilter.CriteriaRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AdvancedFilter. تحصل على نطاق المعايير لهذا الفلتر المتقدم"
type: docs
url: /ar/net/aspose.cells/advancedfilter/criteriarange/
---
## AdvancedFilter.CriteriaRange property

يحصل على نطاق المعايير لهذا الفلتر المتقدم.

```csharp
public string CriteriaRange { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AdvancedFilterPropertyCriteriaRangeDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // املأ بيانات عينة لنطاق القائمة
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["A2"].PutValue("Food");
            sheet.Cells["B2"].PutValue(120);
            sheet.Cells["A3"].PutValue("Transport");
            sheet.Cells["B3"].PutValue(80);
            sheet.Cells["A4"].PutValue("Food");
            sheet.Cells["B4"].PutValue(150);

            // ملء معايير عينة (سيستخدم الفلتر هذه عند التطبيق)
            sheet.Cells["D1"].PutValue("Category");
            sheet.Cells["D2"].PutValue("Food");

            try
            {
                // الحصول على كائن AdvancedFilter للورقة
                AdvancedFilter filter = sheet.GetAdvancedFilter();

                // خصائص ListRange و CriteriaRange و CopyToRange للقراءة فقط.
                // عرض النطاقات المحددة تلقائيًا.
                Console.WriteLine("List Range:    " + filter.ListRange);
                Console.WriteLine("Criteria Range:" + filter.CriteriaRange);
                Console.WriteLine("Copy To Range: " + filter.CopyToRange);

                // حفظ المصنف (اختياري، فقط لإظهار إمكانية إنشاء الملف)
                workbook.Save("AdvancedFilterCriteriaRangeDemo.xlsx");
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

* class [AdvancedFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


