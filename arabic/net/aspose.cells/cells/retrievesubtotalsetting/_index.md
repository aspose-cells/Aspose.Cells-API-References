---
title: "Cells.RetrieveSubtotalSetting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تسترجع إعداد التجميعات الفرعية للنطاق"
type: docs
url: /ar/net/aspose.cells/cells/retrievesubtotalsetting/
---
## Cells.RetrieveSubtotalSetting method

يسترجع إعدادات المجاميع الفرعية للنطاق.

```csharp
public SubtotalSetting RetrieveSubtotalSetting(CellArea ca)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | CellArea | النطاق |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodRetrieveSubtotalSettingWithCellAreaDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة للتجميعات الفرعية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue(i % 2 == 0 ? "Group1" : "Group2");
                worksheet.Cells["B" + i].PutValue(i * 100);
            }

            // إنشاء تجميعات فرعية
            CellArea area = CellArea.CreateCellArea("A1", "B10");
            worksheet.Cells.Subtotal(area, 0, ConsolidationFunction.Sum, new int[] { 1 });

            // استرجاع إعدادات التجميعات الفرعية
            SubtotalSetting setting = worksheet.Cells.RetrieveSubtotalSetting(area);

            // إخراج الإعدادات
            Console.WriteLine("GroupBy: " + setting.GroupBy);
            Console.WriteLine("Function: " + setting.SubtotalFunction);
            Console.WriteLine("SummaryBelowData: " + setting.SummaryBelowData);
            Console.WriteLine("TotalList: " + string.Join(",", setting.TotalList));
        }
    }
}
```

### انظر أيضًا

* class [SubtotalSetting](../../subtotalsetting/)
* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


