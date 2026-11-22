---
title: "CustomFilterCollection.And"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CustomFilterCollection. تشير إلى ما إذا كان للمعيارين علاقة AND"
type: docs
url: /ar/net/aspose.cells/customfiltercollection/and/
---
## CustomFilterCollection.And property

يشير إلى ما إذا كان للمعيارين علاقة "و".

```csharp
public bool And { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CustomFilterCollectionPropertyAndDemo
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
                // إنشاء CustomFilterCollection جديد
                CustomFilterCollection filters = new CustomFilterCollection();

                // عرض القيمة الافتراضية لخاصية And
                Console.WriteLine($"Default And property value: {filters.And}");

                // تعيين خاصية And إلى true
                filters.And = true;
                Console.WriteLine($"After setting to true, And property value: {filters.And}");

                // تعيين خاصية And إلى false
                filters.And = false;
                Console.WriteLine($"After setting to false, And property value: {filters.And}");

                // احفظ المصنف
                workbook.Save("CustomFilterCollectionAndDemo.xlsx");
                Console.WriteLine("CustomFilterCollection And property demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating And property: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [CustomFilterCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


