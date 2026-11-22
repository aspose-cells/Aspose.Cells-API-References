---
title: "فئة SubtotalSetting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.SubtotalSetting. تمثل إعداد التجميع الفرعي"
type: docs
url: /ar/net/aspose.cells/subtotalsetting/
---
## SubtotalSetting class

يمثل إعداد الإجمال الفرعي.

```csharp
public class SubtotalSetting
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [GroupBy](../../aspose.cells/subtotalsetting/groupby/) { get; } | الحقل لتجميعه، كإزاحة عددية تبدأ من الصفر |
| [SubtotalFunction](../../aspose.cells/subtotalsetting/subtotalfunction/) { get; } | دالة التجميع الفرعي. |
| [SummaryBelowData](../../aspose.cells/subtotalsetting/summarybelowdata/) { get; } | يشير إلى ما إذا كان يتم إضافة ملخص أسفل البيانات. |
| [TotalList](../../aspose.cells/subtotalsetting/totallist/) { get; } | مصفوفة من إزاحات الحقول ذات القاعدة الصفرية، تشير إلى الحقول التي تُضاف إليها المجاميع الفرعية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassSubtotalSettingDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إضافة بيانات عينة إلى ورقة العمل
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["A2"].PutValue("Group A");
                worksheet.Cells["A3"].PutValue("Group B");
                worksheet.Cells["A4"].PutValue("Group A");
                worksheet.Cells["A5"].PutValue("Group B");
                worksheet.Cells["B2"].PutValue(100);
                worksheet.Cells["B3"].PutValue(200);
                worksheet.Cells["B4"].PutValue(300);
                worksheet.Cells["B5"].PutValue(400);

                // حدد مساحة الخلية للمجاميع الفرعية
                CellArea area = CellArea.CreateCellArea("A1", "B5");

                // طبق المجاميع الفرعية على البيانات
                worksheet.Cells.Subtotal(
                    area,
                    0, // Group by first column (Category)
                    ConsolidationFunction.Sum,
                    new int[] { 1 }, // Subtotal on second column (Value)
                    true,
                    true,
                    true);

                // استرجع SubtotalSetting من ورقة العمل
                SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);

                // اعرض خصائص SubtotalSetting
                Console.WriteLine("Subtotal Setting Properties:");
                Console.WriteLine($"GroupBy field index: {subtotalSetting.GroupBy}");
                Console.WriteLine($"Subtotal Function: {subtotalSetting.SubtotalFunction}");
                Console.WriteLine($"TotalList contains column index: {subtotalSetting.TotalList[0]}");
                Console.WriteLine($"Summary Below Data: {subtotalSetting.SummaryBelowData}");

                // احفظ المصنف
                workbook.Save("SubtotalSettingDemo.xlsx");
                Console.WriteLine("SubtotalSetting demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SubtotalSetting: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


