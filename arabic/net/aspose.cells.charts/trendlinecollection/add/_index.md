---
title: "TrendlineCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة TrendlineCollection. تضيف كائن Trendline إلى هذه المجموعة بالنوع المحدد"
type: docs
url: /ar/net/aspose.cells.charts/trendlinecollection/add/
---
## Add(TrendlineType) {#add}

تضيف كائن [`Trendline`](../../trendline/) إلى هذه المجموعة بالنوع المحدد.

```csharp
public int Add(TrendlineType type)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | TrendlineType | نوع Trendline. |

### قيمة الإرجاع

[`Trendline`](../../trendline/) object index.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlineCollectionMethodAddWithTrendlineTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["B3"].PutValue(4);
            worksheet.Cells["B4"].PutValue(8);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // إضافة بيانات السلسلة
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // أضف خط اتجاه أسي إلى السلسلة الأولى
            chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);

            // احفظ المصنف
            workbook.Save("TrendlineCollectionMethodAddWithTrendlineTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TrendlineType](../../trendlinetype/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(TrendlineType, string) {#add_1}

تضيف كائن [`Trendline`](../../trendline/) إلى هذه المجموعة بالنوع والاسم المحددين.

```csharp
public int Add(TrendlineType type, string name)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | TrendlineType | نوع Trendline. |
| name | String | اسم Trendline. |

### قيمة الإرجاع

[`Trendline`](../../trendline/) object index.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlineCollectionMethodAddWithTrendlineTypeStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("X Values");
            sheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
            }

            // إنشاء مخطط
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // أضف سلسلة واضبط البيانات
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries[0].XValues = "A2:A10";
            chart.NSeries[0].Name = "Data Series";

            // أضف خط اتجاه باستخدام TrendlineType والاسم
            chart.NSeries[0].TrendLines.Add(TrendlineType.Logarithmic, "Logarithmic Trend");
            
            // اضبط بعض خصائص خط الاتجاه
            Trendline trendline = chart.NSeries[0].TrendLines[0];
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = true;
            
            workbook.Save("TrendlineDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TrendlineType](../../trendlinetype/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


