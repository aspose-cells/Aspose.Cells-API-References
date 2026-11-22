---
title: "Metered.GetConsumptionCredit"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Metered. تحصل على رصيد الاستهلاك"
type: docs
url: /ar/net/aspose.cells/metered/getconsumptioncredit/
---
## Metered.GetConsumptionCredit method

يحصل على رصيد الاستهلاك

```csharp
public static decimal GetConsumptionCredit()
```

### قيمة الإرجاع

كمية الاستهلاك

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodGetConsumptionCreditDemo
    {
        public static void Run()
        {
            // إنشاء نسخة من فئة Metered
            Metered metered = new Metered();

            try
            {
                // استدعاء طريقة GetConsumptionCredit كطريقة ثابتة
                decimal consumptionCredit = Metered.GetConsumptionCredit();
                
                // اعرض النتيجة
                Console.WriteLine($"Current consumption credit: {consumptionCredit}");
                
                // إنشاء مصنف بسيط لتوضيح التأثير (على الرغم من أن GetConsumptionCredit لا يعدل المصنف)
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                
                // إضافة معلومات رصيد الاستهلاك إلى ورقة العمل
                worksheet.Cells["A1"].PutValue("Consumption Credit:");
                worksheet.Cells["B1"].PutValue(consumptionCredit.ToString());
                
                // احفظ المصنف
                workbook.Save("MeteredGetConsumptionCreditDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error getting consumption credit: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


