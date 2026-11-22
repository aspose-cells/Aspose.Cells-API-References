---
title: "AdvancedFilter.CopyToRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية AdvancedFilter. تحصل على النطاق الذي يتم نسخ نتيجة هذا الفلتر المتقدم إليه"
type: docs
url: /ar/net/aspose.cells/advancedfilter/copytorange/
---
## AdvancedFilter.CopyToRange property

يحصل على النطاق الذي يتم نسخ نتيجة هذا الفلتر المتقدم إليه.

```csharp
public string CopyToRange { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AdvancedFilterPropertyCopyToRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // احصل على ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1.5);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(0.8);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(1.2);

            // إضافة نطاق المعايير
            worksheet.Cells["D1"].PutValue("Product");
            worksheet.Cells["D2"].PutValue("Apple");

            try
            {
                // احصل على نسخة AdvancedFilter من ورقة العمل
                AdvancedFilter advancedFilter = worksheet.GetAdvancedFilter();

                // عرض قيمة خاصية CopyToRange
                Console.WriteLine("CopyToRange value: " + advancedFilter.CopyToRange);

                // احفظ المصنف
                workbook.Save("CopyToRangeDemo.xlsx");
                Console.WriteLine("CopyToRange demonstration completed successfully.");
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


