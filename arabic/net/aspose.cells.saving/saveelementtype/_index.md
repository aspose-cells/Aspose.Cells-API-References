---
title: "تعداد SaveElementType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Saving.SaveElementType. يمثل نوع العناصر التي يجب حفظها."
type: docs
url: /ar/net/aspose.cells.saving/saveelementtype/
---
## SaveElementType enumeration

يمثل نوع العناصر التي يجب حفظها.

```csharp
public enum SaveElementType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| All | `251658239` | جميع البيانات. |
| Chart | `256` | الرسوم البيانية فقط. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Saving;
    using System;

    public class SavingClassSaveElementTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إضافة بعض البيانات النموذجية لتوضيح عملية الحفظ
                worksheet.Cells["A1"].PutValue("Sample Data");
                worksheet.Cells["B1"].PutValue(12345);

                // إنشاء رسم بياني لتوضيح نوع عنصر حفظ الرسم البياني
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("A1:B1", true);

                // توضيح استخدام قيم تعداد SaveElementType
                SaveElementType chartType = SaveElementType.Chart;
                SaveElementType allType = SaveElementType.All;

                Console.WriteLine($"Chart SaveElementType value: {chartType}");
                Console.WriteLine($"All SaveElementType value: {allType}");

                // حفظ المصنف مع جميع العناصر
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
                workbook.Save("SaveElementTypeDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved successfully with all elements");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SaveElementType: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


