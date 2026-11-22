---
title: "FontConfigs.IsFontAvailable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FontConfigs. تشير إلى ما إذا كان الخط متاحًا"
type: docs
url: /ar/net/aspose.cells/fontconfigs/isfontavailable/
---
## FontConfigs.IsFontAvailable method

حدد ما إذا كان الخط متاحًا.

```csharp
public static bool IsFontAvailable(string fontName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fontName | String | اسم الخط |

### قيمة الإرجاع

صحيح إذا كان الخط متاحًا، وإلا خطأ.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodIsFontAvailableWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // اختبار أسماء الخطوط للتحقق من التوفر
            string[] testFonts = { "Arial", "Times New Roman", "NonExistentFont" };

            try
            {
                foreach (string fontName in testFonts)
                {
                    // استدعاء طريقة IsFontAvailable مع اسم الخط
                    bool isAvailable = FontConfigs.IsFontAvailable(fontName);

                    // اعرض النتيجة
                    Console.WriteLine($"Font '{fontName}' is available: {isAvailable}");

                    // كتابة النتيجة إلى ورقة العمل
                    int row = worksheet.Cells.MaxDataRow + 1;
                    worksheet.Cells[row, 0].PutValue($"Font '{fontName}' available:");
                    worksheet.Cells[row, 1].PutValue(isAvailable);
                }

                Console.WriteLine("Method executed successfully with parameters (String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsFontAvailable method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("FontConfigsMethodIsFontAvailableWithStringDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


