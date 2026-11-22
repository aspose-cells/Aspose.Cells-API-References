---
title: "SeriesCollection.SwapSeries"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SeriesCollection. تغير مباشرةً ترتيب السلسلتين"
type: docs
url: /ar/net/aspose.cells.charts/seriescollection/swapseries/
---
## SeriesCollection.SwapSeries method

يغيّر مباشرة ترتيب السلسلتين.

```csharp
public void SwapSeries(int sourceIndex, int destIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceIndex | Int32 | الفهرس الحالي |
| destIndex | Int32 | فهرس الوجهة |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodSwapSeriesWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            
            worksheet.Cells["B1"].PutValue("Series 2");
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(10);
            worksheet.Cells["B4"].PutValue(15);
            
            worksheet.Cells["C1"].PutValue("Series 3");
            worksheet.Cells["C2"].PutValue(8);
            worksheet.Cells["C3"].PutValue(16);
            worksheet.Cells["C4"].PutValue(24);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("A1:C4", true);
            
            // احصل على مجموعة السلاسل
            Aspose.Cells.Charts.SeriesCollection sc = chart.NSeries;
            
            // طباعة أسماء السلاسل الأصلية
            Console.WriteLine("Original Series Order:");
            for (int i = 0; i < sc.Count; i++)
            {
                Console.WriteLine($"Series {i}: {sc[i].Name}");
            }
            
            // تبديل السلسلة 0 و 1
            sc.SwapSeries(0, 1);
            Console.WriteLine("\nAfter swapping series 0 and 1:");
            for (int i = 0; i < sc.Count; i++)
            {
                Console.WriteLine($"Series {i}: {sc[i].Name}");
            }
            
            // تبديل السلسلة 2 و 0
            sc.SwapSeries(2, 0);
            Console.WriteLine("\nAfter swapping series 2 and 0:");
            for (int i = 0; i < sc.Count; i++)
            {
                Console.WriteLine($"Series {i}: {sc[i].Name}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


