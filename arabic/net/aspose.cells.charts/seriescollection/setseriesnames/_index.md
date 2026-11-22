---
title: "SeriesCollection.SetSeriesNames"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SeriesCollection. تعيين أسماء جميع السلاسل في المخطط"
type: docs
url: /ar/net/aspose.cells.charts/seriescollection/setseriesnames/
---
## SeriesCollection.SetSeriesNames method

يضبط أسماء جميع السلاسل في المخطط.

```csharp
public void SetSeriesNames(int startIndex, string area, bool isVertical)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | Int32 | فهرس السلسلة الأولى التي تريد تعيين اسمها. |
| منطقة | String | يحدد المنطقة لاسم السلسلة. |
| isVertical | منطقي | &gt;يحدد ما إذا كان سيتم رسم السلسلة من نطاق قيم الخلايا حسب الصف أو حسب العمود. |

### ملاحظات

إذا كان فهرس البداية أكبر من عدد السلاسل، فسيتم الإرجاع ولن يحدث شيء. إذا تم تعيين البيانات على خلايا متجاورة، استخدم النقطتين للفصل بينها. على سبيل المثال، $C$2:$C$5. إذا تم تعيين البيانات على خلايا متجاورة، استخدم الفاصلة للفصل بينها. على سبيل المثال، ($C$2,$D$5).

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesCollectionMethodSetSeriesNamesWithInt32StringBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Q1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["C1"].PutValue("Q2");
            worksheet.Cells["C2"].PutValue(120);
            worksheet.Cells["C3"].PutValue(180);
            worksheet.Cells["C4"].PutValue(220);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // الحصول على مجموعة سلاسل المخطط
            SeriesCollection seriesCollection = chart.NSeries;

            try
            {
                // استدعِ SetSeriesNames مع المعلمات (startIndex: 0, area: "A2:A4", isVertical: true)
                seriesCollection.SetSeriesNames(0, "A2:A4", true);

                // إضافة بيانات السلسلة
                seriesCollection.Add("B2:C4", true);

                Console.WriteLine("SetSeriesNames method executed successfully with parameters (Int32, String, Boolean)");
                Console.WriteLine("Series names set from range A2:A4");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetSeriesNames method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("SeriesCollectionMethodSetSeriesNamesWithInt32StringBooleanDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


