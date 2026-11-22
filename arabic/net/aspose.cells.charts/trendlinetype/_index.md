---
title: "التعداد TrendlineType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Charts.TrendlineType. يمثل نوع خط الاتجاه"
type: docs
url: /ar/net/aspose.cells.charts/trendlinetype/
---
## TrendlineType enumeration

يمثل نوع خط الاتجاه.

```csharp
public enum TrendlineType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Exponential | `0` | أسي |
| Linear | `1` | خطّي |
| Logarithmic | `2` | لوغاريتمي |
| MovingAverage | `3` | متوسط متحرك |
| Polynomial | `4` | متعدد الحدود |
| Power | `5` | قوة |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class TrendlineTypeDemo
    {
        public static void TrendlineTypeExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل جديدة إلى كائن Excel
            int sheetIndex = workbook.Worksheets.Add();
            
            // الحصول على مرجع ورقة العمل التي تم إضافتها حديثًا بتمرير sheet index
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // إضافة قيم عينة إلى الخلايا
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // الوصول إلى نسخة المخطط المضاف حديثًا
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة NSeries (مصدر بيانات المخطط) إلى المخطط من الخلية "A1" إلى "B4"
            chart.NSeries.Add("A1:B4", true);
            
            // تعيين مصدر البيانات لبيانات الفئة في NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // إضافة أنواع مختلفة من خطوط الاتجاه إلى المخطط
            AddTrendline(chart, 0, TrendlineType.Linear, "Linear Trendline");
            AddTrendline(chart, 0, TrendlineType.Exponential, "Exponential Trendline");
            AddTrendline(chart, 0, TrendlineType.Logarithmic, "Logarithmic Trendline");
            AddTrendline(chart, 0, TrendlineType.MovingAverage, "Moving Average Trendline");
            AddTrendline(chart, 0, TrendlineType.Polynomial, "Polynomial Trendline");
            AddTrendline(chart, 0, TrendlineType.Power, "Power Trendline");

            // حفظ ملف Excel
            workbook.Save("TrendlineTypeExample.xlsx");
        }

        private static void AddTrendline(Chart chart, int seriesIndex, TrendlineType trendlineType, string trendlineName)
        {
            // إضافة خط اتجاه من النوع المحدد إلى السلسلة المحددة
            int index = chart.NSeries[seriesIndex].TrendLines.Add(trendlineType);
            Trendline trendline = chart.NSeries[seriesIndex].TrendLines[index];
            
            // تعيين الاسم المخصص لخط الاتجاه
            trendline.Name = trendlineName;
            
            // عرض المعادلة على المخطط
            trendline.DisplayEquation = true;
            
            // عرض قيمة R-مربعة على المخطط
            trendline.DisplayRSquared = true;
            
            // تعيين لون خط الاتجاه
            trendline.Color = Color.Red;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


