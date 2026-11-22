---
title: "تعداد SignificantDigitsType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.SignificantDigitsType. يمثل نوع الأرقام ذات الدقة المهمة لإخراج القيم الرقمية"
type: docs
url: /ar/net/aspose.cells/significantdigitstype/
---
## SignificantDigitsType enumeration

يمثل نوع الأرقام ذات الدقة المهمة لإخراج القيم العددية.

```csharp
public enum SignificantDigitsType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Digits15 | `0` | 15-رقم |
| G17 | `1` | 17-رقم عن طريق تنسيق القيمة باستخدام "G17". |
| Rounding17 | `2` | 17-رقم عن طريق تقريب القيمة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassSignificantDigitsTypeDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد للعرض
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // عرض استخدام كل قيمة من تعداد SignificantDigitsType
                SignificantDigitsType[] types = {
                    SignificantDigitsType.Digits15,
                    SignificantDigitsType.G17,
                    SignificantDigitsType.Rounding17
                };

                foreach (SignificantDigitsType type in types)
                {
                    // تعيين نوع الأرقام ذات الدقة المهمة لدفتر العمل
                    workbook.Settings.SignificantDigitsType = type;

                    // عرض الإعداد الحالي
                    Console.WriteLine($"Current SignificantDigitsType: {type} (Value: {(int)type})");

                    // إضافة قيمة نموذجية لتوضيح الإعداد
                    worksheet.Cells["A1"].PutValue(123.4567890123456789);

                    // حفظ دفتر العمل بالإعداد الحالي
                    string fileName = $"SignificantDigitsType_{type}.xlsx";
                    workbook.Save(fileName);
                    Console.WriteLine($"Workbook saved with {type} setting as {fileName}");
                }

                Console.WriteLine("All SignificantDigitsType demonstrations completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating SignificantDigitsType: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


