---
title: "Series.IsVerticalValues"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Series. تشير إلى ما إذا كان مصدر البيانات عموديًا"
type: docs
url: /ar/net/aspose.cells.charts/series/isverticalvalues/
---
## Series.IsVerticalValues property

يشير إلى ما إذا كان مصدر البيانات عموديًا.

```csharp
public bool IsVerticalValues { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsVerticalValuesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Cat " + (i-1));
                worksheet.Cells["B" + i].PutValue(i * 10);
            }

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة سلسلة بقيم عمودية
            chart.NSeries.Add("A1:B10", true);
            
            // عرض خاصية IsVerticalValues (للقراءة فقط)
            Console.WriteLine("IsVerticalValues for first series: " + chart.NSeries[0].IsVerticalValues);
            
            // لتغيير الاتجاه، نحتاج إلى إعادة إنشاء السلسلة بمعلمات مختلفة
            chart.NSeries.Clear();
            chart.NSeries.Add("A1:B10", false);
            Console.WriteLine("IsVerticalValues after recreation: " + chart.NSeries[0].IsVerticalValues);
        }
    }
}
```

### انظر أيضًا

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


