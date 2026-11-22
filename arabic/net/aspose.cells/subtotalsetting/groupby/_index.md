---
title: "SubtotalSetting.GroupBy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SubtotalSetting. الحقل لتجميعه كإزاحة عدد صحيح يبدأ من الصفر"
type: docs
url: /ar/net/aspose.cells/subtotalsetting/groupby/
---
## SubtotalSetting.GroupBy property

الحقل لتجميعه، كإزاحة عددية تبدأ من الصفر

```csharp
public int GroupBy { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SubtotalSettingPropertyGroupByDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
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

            try
            {
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

                // استرجع إعداد subtotal للوصول إلى خاصية GroupBy
                SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);

                // اعرض قيمة خاصية GroupBy
                Console.WriteLine("GroupBy field index: " + subtotalSetting.GroupBy);

                // احفظ المصنف
                workbook.Save("GroupByDemo.xlsx");
                Console.WriteLine("Subtotal with GroupBy demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


