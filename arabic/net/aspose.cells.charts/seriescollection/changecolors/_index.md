---
title: "SeriesCollection.ChangeColors"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SeriesCollection. تعيين لوحة ألوان أحادية اللون لسلسلة المخطط"
type: docs
url: /ar/net/aspose.cells.charts/seriescollection/changecolors/
---
## SeriesCollection.ChangeColors method

ضبط لوحة ألوان أحادية اللون لسلاسل المخطط.

```csharp
public void ChangeColors(ChartColorPaletteType type)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | ChartColorPaletteType | النوع أحادي اللون. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodChangeColorsWithChartColorPaletDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            // املأ بعض البيانات للمخطط
            ws.Cells["A1"].PutValue("Category");
            ws.Cells["A2"].PutValue("Jan");
            ws.Cells["A3"].PutValue("Feb");
            ws.Cells["A4"].PutValue("Mar");

            ws.Cells["B1"].PutValue("Series1");
            ws.Cells["B2"].PutValue(10);
            ws.Cells["B3"].PutValue(20);
            ws.Cells["B4"].PutValue(30);

            ws.Cells["C1"].PutValue("Series2");
            ws.Cells["C2"].PutValue(15);
            ws.Cells["C3"].PutValue(25);
            ws.Cells["C4"].PutValue(35);

            // أضف مخطط عمودي
            int chartIdx = ws.Charts.Add(ChartType.Column, 6, 0, 20, 10);
            Chart chart = ws.Charts[chartIdx];

            // حدد نطاق البيانات للسلسلة
            chart.NSeries.Add("B1:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احصل على مجموعة السلاسل
            SeriesCollection seriesColl = chart.NSeries;

            try
            {
                // غيّر لوحة ألوان جميع السلاسل في المجموعة.
                // استخدم تحويلًا رقميًا إلى قيمة تعداد صالحة (مثال: 0) لتجنب أسماء أعضاء التعداد المعتمدة.
                seriesColl.ChangeColors((ChartColorPaletteType)0);

                Console.WriteLine("ChangeColors method invoked successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error invoking ChangeColors: {ex.Message}");
            }

            // احفظ دفتر العمل للتحقق من النتيجة
            workbook.Save("SeriesCollection_ChangeColors_Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ChartColorPaletteType](../../chartcolorpalettetype/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


