---
title: "الفئة ChartPointCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Charts.ChartPointCollection. تمثل مجموعة تحتوي على جميع النقاط في سلسلة واحدة"
type: docs
url: /ar/net/aspose.cells.charts/chartpointcollection/
---
## ChartPointCollection class

يمثل مجموعة تحتوي على جميع النقاط في سلسلة واحدة.

```csharp
public class ChartPointCollection : IEnumerable
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.cells.charts/chartpointcollection/count/) { get; } | يحصل على عدد نقاط المخطط. |
| [Item](../../aspose.cells.charts/chartpointcollection/item/) { get; } | يحصل على العنصر [`ChartPoint`](../chartpoint/) في الفهرس المحدد داخل السلسلة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Clear](../../aspose.cells.charts/chartpointcollection/clear/)() | إزالة جميع إعدادات نقاط المخطط. |
| [GetEnumerator](../../aspose.cells.charts/chartpointcollection/getenumerator/)() | يرجع مُعدِّدًا لكامل `ChartPointCollection`. |
| [RemoveAt](../../aspose.cells.charts/chartpointcollection/removeat/)(int) | يزيل النقطة في الفهرس الخاص بالسلسلة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointCollectionDemo
    {
        public static void ChartPointCollectionExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();

            // الحصول على مرجع ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة قيم عينة إلى الخلايا
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.PieExploded, 5, 0, 25, 10);

            // الوصول إلى نسخة المخطط المضاف حديثًا
            Chart chart = worksheet.Charts[chartIndex];

            // إضافة NSeries (مصدر بيانات المخطط) إلى المخطط من الخلية "A1" إلى "B3"
            chart.NSeries.Add("A1:B3", true);

            // إظهار تسميات البيانات 
            chart.NSeries[0].DataLabels.ShowValue = true;

            // الوصول إلى ChartPointCollection
            ChartPointCollection points = chart.NSeries[0].Points;

            // التكرار عبر النقاط في المجموعة
            for (int i = 0; i < points.Count; i++)
            {
                // الحصول على نقطة البيانات
                ChartPoint point = points[i];
                
                // ضبط انفجار الفطيرة
                point.Explosion = 15;
                
                // ضبط لون الحدود
                point.Border.Color = System.Drawing.Color.Red;
            }

            // حفظ ملف Excel
            workbook.Save("ChartPointCollectionExample.xlsx");
            workbook.Save("ChartPointCollectionExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


