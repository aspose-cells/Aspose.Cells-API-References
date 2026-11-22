---
title: "Metered.GetConsumptionQuantity"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Metered. تحصل على حجم ملف الاستهلاك"
type: docs
url: /ar/net/aspose.cells/metered/getconsumptionquantity/
---
## Metered.GetConsumptionQuantity method

يحصل على حجم ملف الاستهلاك

```csharp
public static decimal GetConsumptionQuantity()
```

### قيمة الإرجاع

كمية الاستهلاك

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodGetConsumptionQuantityDemo
    {
        public static void Run()
        {
            // إنشاء نسخة metered
            Metered metered = new Metered();

            try
            {
                // تعيين المفاتيح المقاسة (استبدل بالمفاتيح الفعلية في الاستخدام الحقيقي)
                metered.SetMeteredKey("your-public-key", "your-private-key");

                // الحصول على كمية الاستهلاك
                decimal consumptionQuantity = Metered.GetConsumptionQuantity();

                // اعرض النتيجة
                Console.WriteLine($"Consumption Quantity: {consumptionQuantity}");

                // إنشاء مصنف لتوضيح الاستخدام المقاس
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // إضافة بعض البيانات لإظهار أن المصنف يعمل
                worksheet.Cells["A1"].PutValue("Metered Consumption Demo");
                worksheet.Cells["A2"].PutValue($"Consumption Quantity: {consumptionQuantity}");

                // احفظ المصنف
                workbook.Save("MeteredConsumptionDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in metered operation: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


