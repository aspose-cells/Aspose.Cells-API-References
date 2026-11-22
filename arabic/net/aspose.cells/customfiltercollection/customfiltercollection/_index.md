---
title: "CustomFilterCollection.CustomFilterCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ CustomFilterCollection. ينشئ نسخة جديدة"
type: docs
url: /ar/net/aspose.cells/customfiltercollection/customfiltercollection/
---
## CustomFilterCollection constructor

ينشئ نسخة جديدة.

```csharp
[Obsolete("Use FilterColumn.CustomFilters, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public CustomFilterCollection()
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى تعيين FilterColumn.FilterType إلى FilterType.CustomFilters ثم الحصول على FilterColumn.CustomFilters. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد تعرضت له.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionMethodSharpctorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].Value = "Numbers";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;
            worksheet.Cells["A5"].Value = 40;
            worksheet.Cells["A6"].Value = 50;

            try
            {
                // إنشاء CustomFilterCollection جديد باستخدام المنشئ
                CustomFilterCollection filters = new CustomFilterCollection();

                // عرض القيمة الافتراضية لخاصية And
                Console.WriteLine($"Default And property value: {filters.And}");

                // المنشئ ينشئ مجموعة فارغة
                Console.WriteLine($"Number of filters in collection: {filters.Count}");

                // احفظ المصنف
                workbook.Save("CustomFilterCollectionDemo.xlsx");
                Console.WriteLine("CustomFilterCollection created successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating CustomFilterCollection: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


