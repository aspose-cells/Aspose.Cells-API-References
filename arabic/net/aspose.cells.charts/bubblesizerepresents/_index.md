---
title: "تعداد BubbleSizeRepresents"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Charts.BubbleSizeRepresents. يمثل ما تمثله حجم الفقاعات في مخطط الفقاعات."
type: docs
url: /ar/net/aspose.cells.charts/bubblesizerepresents/
---
## BubbleSizeRepresents enumeration

يمثل ما تمثله حجم الفقاعات في مخطط الفقاعات.

```csharp
public enum BubbleSizeRepresents
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| SizeIsArea | `0` | يمثل قيمة [`BubbleSizes`](../series/bubblesizes/)، والتي هي مساحة الفقاعة. |
| SizeIsWidth | `1` | يمثل قيمة [`BubbleSizes`](../series/bubblesizes/) وهو عرض الفقاعة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class BubbleSizeRepresentsDemo
    {
        public static void BubbleSizeRepresentsExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لمخطط الفقاعات
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["B2"].PutValue(3);
            worksheet.Cells["B3"].PutValue(4);
            worksheet.Cells["C1"].PutValue(5);
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(15);

            // إضافة مخطط فقاعات إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // إضافة سلسلة إلى مخطط الفقاعات
            int seriesIndex = chart.NSeries.Add("A1:C3", true);
            Series series = chart.NSeries[seriesIndex];

            // تعيين قيم X، قيم Y، وأحجام الفقاعات
            series.XValues = "A1:A3";
            series.Values = "B1:B3";
            series.BubbleSizes = "C1:C3";

            // تعيين تمثيل حجم الفقاعات
            series.SizeRepresents = BubbleSizeRepresents.SizeIsArea;

            // احفظ المصنف
            workbook.Save("BubbleSizeRepresentsExample.xlsx");
            workbook.Save("BubbleSizeRepresentsExample.pdf");

            // تعيين تمثيل حجم الفقاعات
            series.SizeRepresents = BubbleSizeRepresents.SizeIsWidth;

            // احفظ المصنف
            workbook.Save("BubbleSizeRepresentsExample2.xlsx");
            workbook.Save("BubbleSizeRepresentsExample2.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


