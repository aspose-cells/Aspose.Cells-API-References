---
title: "SubtotalSetting.SubtotalFunction"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SubtotalSetting. دالة الملخص الفرعي"
type: docs
url: /ar/net/aspose.cells/subtotalsetting/subtotalfunction/
---
## SubtotalSetting.SubtotalFunction property

دالة التجميع الفرعي.

```csharp
public ConsolidationFunction SubtotalFunction { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertySubtotalFunctionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i % 2 == 0 ? "Group A" : "Group B");
                worksheet.Cells["B" + i].PutValue(i * 100);
            }

            // أنشئ إعداد الملخص الفرعي عن طريق الاسترجاع من البيانات الموجودة
            CellArea area = CellArea.CreateCellArea("A1", "B10");
            SubtotalSetting subtotalSetting = worksheet.Cells.RetrieveSubtotalSetting(area);
            
            // قم بتكوين الملخص الفرعي - هذه الخصائص للقراءة فقط في واجهة برمجة التطبيقات الفعلية
            // لذا سنستخدم طريقة Subtotal مباشرةً مع المعلمات
            int groupBy = 0; // Group by first column
            ConsolidationFunction function = ConsolidationFunction.Sum;
            int[] subtotalColumns = new int[] {1}; // Subtotal on second column
            
            // طبق الملخصات الفرعية
            worksheet.Cells.Subtotal(area, groupBy, function, subtotalColumns);

            // تحقق من خاصية SubtotalFunction من الإعداد المسترجع
            Console.WriteLine("Subtotal Function: " + subtotalSetting.SubtotalFunction);
            
            // احفظ المصنف
            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


