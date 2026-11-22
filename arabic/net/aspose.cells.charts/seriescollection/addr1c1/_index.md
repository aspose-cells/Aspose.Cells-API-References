---
title: "SeriesCollection.AddR1C1"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SeriesCollection. تضيف مجموعة Series إلى مخطط"
type: docs
url: /ar/net/aspose.cells.charts/seriescollection/addr1c1/
---
## SeriesCollection.AddR1C1 method

تضيف مجموعة [`Series`](../../series/) إلى مخطط.

```csharp
public int AddR1C1(string area, bool isVertical)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| منطقة | String | يحدد القيم التي سيتم رسم سلسلة البيانات منها |
| isVertical | منطقي | يحدد ما إذا كان سيتم رسم السلسلة من نطاق قيم الخلايا حسب الصف أو حسب العمود. |

### قيمة الإرجاع

إرجاع الفهرس الأول للسلسلة ASeries المضافة في NSeries.

### ملاحظات

إذا تم تعيين البيانات على خلايا متجاورة، استخدم النقطتين للفصل بينها. على سبيل المثال، R[1]C[1]:R[3]C[2]. إذا تم تعيين البيانات على خلايا متجاورة، استخدم الفاصلة للفصل بينها. على سبيل المثال، (R[1]C[1],R[3]C[2]).

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodAddR1C1WithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet wsData = workbook.Worksheets[0];
            wsData.Name = "ChartData";

            // بيانات عينة
            wsData.Cells[0, 0].PutValue(1);
            wsData.Cells[1, 0].PutValue(2);
            wsData.Cells[0, 1].PutValue(3);
            wsData.Cells[1, 1].PutValue(4);

            Worksheet wsChart = workbook.Worksheets[workbook.Worksheets.Add(Aspose.Cells.SheetType.Chart)];
            wsChart.Name = "ChartSheet";

            int chartIndex = wsChart.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 0, 0, 15, 15);
            Aspose.Cells.Charts.Chart chart = wsChart.Charts[chartIndex];

            // استخدام AddR1C1 مع معلمات String و Boolean
            int seriesIndex = chart.NSeries.AddR1C1("ChartData!R1C2:R2C2", true);
            Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];
            series.XValues = "ChartData!R1C1:R2C1";

            workbook.Save("SeriesCollectionAddR1C1Demo.xlsx", Aspose.Cells.SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


