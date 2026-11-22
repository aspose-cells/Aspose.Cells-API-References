---
title: "SeriesCollection.RemoveAt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SeriesCollection. إزالة سلسلة عند الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells.charts/seriescollection/removeat/
---
## SeriesCollection.RemoveAt method

إزالة سلسلة عند الفهرس المحدد.

```csharp
public void RemoveAt(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | الفهرس. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesCollectionMethodRemoveAtWithInt32Demo
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
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B1:B4", true);
            chart.NSeries.Add("C1:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // استدعِ RemoveAt لإزالة السلسلة الأولى (الفهرس 0)
                chart.NSeries.RemoveAt(0);
                
                Console.WriteLine("Series at index 0 removed successfully");
                
                // تحقق من عدد السلاسل المتبقية
                Console.WriteLine($"Remaining series count: {chart.NSeries.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("SeriesCollectionMethodRemoveAtWithInt32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


