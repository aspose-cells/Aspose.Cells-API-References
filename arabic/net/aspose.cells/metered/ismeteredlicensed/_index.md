---
title: "Metered.IsMeteredLicensed"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Metered. تحقق مما إذا كان metered مرخصًا"
type: docs
url: /ar/net/aspose.cells/metered/ismeteredlicensed/
---
## Metered.IsMeteredLicensed method

تحقق مما إذا كان Metered مرخصًا

```csharp
public static bool IsMeteredLicensed()
```

### قيمة الإرجاع

صحيح أم خطأ

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodIsMeteredLicensedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نسخة Metered
            Metered metered = new Metered();

            try
            {
                // تحقق مما إذا كان ترخيص metered مطبقًا
                bool isLicensed = Metered.IsMeteredLicensed();

                // اعرض النتيجة
                Console.WriteLine($"Is Metered Licensed: {isLicensed}");

                // أضف النتيجة إلى ورقة العمل
                worksheet.Cells["A1"].PutValue("Is Metered Licensed:");
                worksheet.Cells["B1"].PutValue(isLicensed);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsMeteredLicensed method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("MethodIsMeteredLicensedDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


