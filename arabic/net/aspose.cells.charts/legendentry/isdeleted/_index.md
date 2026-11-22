---
title: "LegendEntry.IsDeleted"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LegendEntry. تحصل وتضبط ما إذا كان إدخال الوسيلة الإيضاحية محذوفًا"
type: docs
url: /ar/net/aspose.cells.charts/legendentry/isdeleted/
---
## LegendEntry.IsDeleted property

يحصل ويضبط ما إذا كان إدخال الوسيلة محذوفًا.

```csharp
public bool IsDeleted { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendEntryPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // احصل على أول إدخال للوسيلة الإيضاحية
            LegendEntry legendEntry = chart.Legend.LegendEntries[0];

            // توضيح خاصية IsDeleted
            Console.WriteLine("Legend entry initially deleted? " + legendEntry.IsDeleted);
            
            // حذف إدخال الوسيلة الإيضاحية
            legendEntry.IsDeleted = true;
            Console.WriteLine("Legend entry after deletion? " + legendEntry.IsDeleted);

            // استعادة إدخال الوسيلة الإيضاحية
            legendEntry.IsDeleted = false;
            Console.WriteLine("Legend entry after restoration? " + legendEntry.IsDeleted);

            // احفظ المصنف
            workbook.Save("LegendEntryIsDeletedDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [LegendEntry](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


