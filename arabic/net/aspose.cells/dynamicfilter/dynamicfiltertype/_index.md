---
title: "DynamicFilter.DynamicFilterType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DynamicFilter. تحصل وتعيّن نوع هذا المرشح الديناميكي"
type: docs
url: /ar/net/aspose.cells/dynamicfilter/dynamicfiltertype/
---
## DynamicFilter.DynamicFilterType property

يحصل ويضبط نوع هذا الفلتر الديناميكي.

```csharp
public DynamicFilterType DynamicFilterType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterPropertyDynamicFilterTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة مع تواريخ
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 15));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 20));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 10));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 5));

            try
            {
                // إنشاء مرشح تلقائي
                worksheet.AutoFilter.Range = "A1:A5";

                // طبق مرشحًا ديناميكيًا لتواريخ مارس
                worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

                // احصل على كائن DynamicFilter
                DynamicFilter filter = (DynamicFilter)worksheet.AutoFilter.FilterColumns[0].Filter;

                // اعرض قيمة DynamicFilterType الحالية
                Console.WriteLine("Current DynamicFilterType: " + filter.DynamicFilterType);

                // غيّر نوع المرشح لعرض تواريخ أبريل
                filter.DynamicFilterType = DynamicFilterType.April;

                // اعرض قيمة DynamicFilterType المحدثة
                Console.WriteLine("Updated DynamicFilterType: " + filter.DynamicFilterType);

                // تطبيق الفلتر
                worksheet.AutoFilter.Refresh();

                // حفظ النتيجة
                workbook.Save("DynamicFilterTypeDemo.xlsx");
                Console.WriteLine("DynamicFilterType has been demonstrated successfully.");
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

* enum [DynamicFilterType](../../dynamicfiltertype/)
* class [DynamicFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


