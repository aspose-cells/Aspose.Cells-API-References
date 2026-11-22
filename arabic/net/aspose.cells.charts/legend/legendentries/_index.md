---
title: "Legend.LegendEntries"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Legend. يحصل على مجموعة من جميع كائنات LegendEntry في وسيلة الإيضاح المحددة للمخطط. لا يتم دعم إعداد مدخلات الوسيلة لمخطط السطح. لذلك سيعيد null إذا كان نوع المخطط هو مخطط سطح."
type: docs
url: /ar/net/aspose.cells.charts/legend/legendentries/
---
## Legend.LegendEntries property

يحصل على مجموعة من جميع كائنات LegendEntry في وسيلة إيضاح المخطط المحددة. لا يدعم ضبط إدخالات وسيلة الإيضاح للمخطط السطحي. لذلك سيعيد null إذا كان نوع المخطط هو نوع المخطط السطحي.

```csharp
public LegendEntryCollection LegendEntries { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendPropertyLegendEntriesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "B2:B4";

            // الوصول إلى عناصر الأسطورة
            Aspose.Cells.Charts.LegendEntryCollection legendEntries = chart.Legend.LegendEntries;
            
            // احذف مدخل legend الثاني
            legendEntries[1].IsDeleted = true;
            
            // احفظ المصنف
            workbook.Save("LegendEntriesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [LegendEntryCollection](../../legendentrycollection/)
* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


