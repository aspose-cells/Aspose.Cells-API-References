---
title: "SeriesCollection.GetSeriesByOrder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SeriesCollection. تحصل على عنصر Series حسب الترتيب"
type: docs
url: /ar/net/aspose.cells.charts/seriescollection/getseriesbyorder/
---
## SeriesCollection.GetSeriesByOrder method

يحصل على عنصر [`Series`](../../series/) حسب الترتيب.

```csharp
public Series GetSeriesByOrder(int order)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ترتيب | Int32 | ترتيب السلاسل |

### قيمة الإرجاع

عنصر السلسلة

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesCollectionMethodGetSeriesByOrderWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");
            
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["B5"].PutValue(400);
            
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);
            worksheet.Cells["C5"].PutValue(450);

            // إنشاء مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.Add("C2:C5", true);
            chart.NSeries.CategoryData = "A2:A5";

            try
            {
                // احصل على السلسلة الأولى (order = 0)
                Series series = chart.NSeries.GetSeriesByOrder(0);
                
                if (series != null)
                {
                    // عدّل خصائص السلسلة
                    series.Name = "Modified Series 1";
                    series.Shadow = true;
                    
                    Console.WriteLine("Successfully retrieved and modified series with order 0");
                    Console.WriteLine($"Series Name: {series.Name}");
                    Console.WriteLine($"Shadow Enabled: {series.Shadow}");
                }
                
                // احفظ المصنف
                workbook.Save("SeriesCollectionMethodGetSeriesByOrderDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSeriesByOrder method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Series](../../series/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


