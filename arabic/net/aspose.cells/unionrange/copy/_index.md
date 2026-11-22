---
title: "UnionRange.Copy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة UnionRange. نسخ النطاق باستخدام خيارات اللصق الخاصة"
type: docs
url: /ar/net/aspose.cells/unionrange/copy/
---
## UnionRange.Copy method

نسخ النطاق باستخدام خيارات اللصق الخاصة.

```csharp
public void Copy(UnionRange range, PasteOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نطاق | UnionRange | النطاق المصدر. |
| خيارات | PasteOptions | خيارات اللصق الخاص. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangeMethodCopyWithUnionRangePasteOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Source Data");
            worksheet.Cells["B1"].PutValue("Value1");
            worksheet.Cells["A2"].PutValue("More Data");
            worksheet.Cells["B2"].PutValue("Value2");

            try
            {
                // أنشئ UnionRange المصدر
                UnionRange sourceRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(
                    new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

                // أنشئ UnionRange الوجهة
                UnionRange destinationRange = worksheet.Cells.CreateRange("D1:E2").UnionRanges(
                    new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("D1:E2") });

                // أنشئ PasteOptions بإعدادات محددة
                PasteOptions options = new PasteOptions();
                options.PasteType = PasteType.All;
                options.SkipBlanks = true;
                options.Transpose = false;

                // استدعِ طريقة Copy
                sourceRange.Copy(destinationRange, options);

                Console.WriteLine("Copy method executed successfully");
                Console.WriteLine($"Destination range: {destinationRange.RefersTo}");

                // احفظ المصنف
                workbook.Save("UnionRangeCopyDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Copy: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [PasteOptions](../../pasteoptions/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


