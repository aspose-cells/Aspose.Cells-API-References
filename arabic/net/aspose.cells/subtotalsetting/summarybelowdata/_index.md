---
title: "SubtotalSetting.SummaryBelowData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SubtotalSetting. تشير إلى ما إذا كان يتم إضافة ملخص أسفل البيانات"
type: docs
url: /ar/net/aspose.cells/subtotalsetting/summarybelowdata/
---
## SubtotalSetting.SummaryBelowData property

يشير إلى ما إذا كان يتم إضافة ملخص أسفل البيانات.

```csharp
public bool SummaryBelowData { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertySummaryBelowDataDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("A");
            worksheet.Cells["A4"].PutValue("B");
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // أنشئ منطقة خلايا للملخصات الفرعية
            CellArea area = CellArea.CreateCellArea("A1", "B5");

            // طبق الملخصات الفرعية باستخدام طريقة Cells.Subtotal مع جميع المعلمات المطلوبة
            worksheet.Cells.Subtotal(
                area, 
                0, 
                ConsolidationFunction.Sum, 
                new int[] { 1 }, 
                false, 
                false, 
                false);  // summaryBelowData parameter

            // استرجع الإعداد للتحقق من SummaryBelowData
            SubtotalSetting retrievedSetting = worksheet.Cells.RetrieveSubtotalSetting(area);
            
            // أخرج قيمة خاصية SummaryBelowData
            Console.WriteLine("SummaryBelowData: " + retrievedSetting.SummaryBelowData);
        }
    }
}
```

### انظر أيضًا

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


