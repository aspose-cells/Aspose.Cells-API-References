---
title: "SubtotalSetting.TotalList"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SubtotalSetting. مصفوفة من إزاحات الحقول التي تبدأ من الصفر تشير إلى الحقول التي تُضاف إليها الملخصات الفرعية"
type: docs
url: /ar/net/aspose.cells/subtotalsetting/totallist/
---
## SubtotalSetting.TotalList property

مصفوفة من إزاحات الحقول ذات القاعدة الصفرية، تشير إلى الحقول التي تُضاف إليها المجاميع الفرعية.

```csharp
public int[] TotalList { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SubtotalSettingPropertyTotalListDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إعداد بيانات العينة
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // أنشئ وطبق الملخص الفرعي
            CellArea area = CellArea.CreateCellArea("A1", "B5");
            worksheet.Cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 1 }, true, true, true);

            // استرجع إعداد الملخص الفرعي لتوضيح استخدام TotalList
            SubtotalSetting subtotal = worksheet.Cells.RetrieveSubtotalSetting(area);
            Console.WriteLine("TotalList contains column index: " + subtotal.TotalList[0]);
            
            // احفظ المصنف
            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SubtotalSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


