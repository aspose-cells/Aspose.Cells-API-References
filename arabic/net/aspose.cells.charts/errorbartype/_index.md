---
title: "تعداد ErrorBarType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Charts.ErrorBarType تعداد. يمثل نوع مقدار شريط الخطأ"
type: docs
url: /ar/net/aspose.cells.charts/errorbartype/
---
## ErrorBarType enumeration

يمثل نوع مقدار شريط الخطأ.

```csharp
public enum ErrorBarType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Custom | `0` | نوع قيمة InnerCustom. |
| FixedValue | `1` | نوع قيمة ثابتة. |
| Percent | `2` | نوع النسبة المئوية |
| StDev | `3` | نوع الانحراف المعياري. |
| StError | `4` | نوع الخطأ المعياري. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ErrorBarTypeDemo
    {
        public static void ErrorBarTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // أضف بعض البيانات التجريبية
            cells["A1"].PutValue(2);
            cells["A2"].PutValue(5);
            cells["A3"].PutValue(3);
            cells["A4"].PutValue(6);
            cells["B1"].PutValue(4);
            cells["B2"].PutValue(3);
            cells["B3"].PutValue(6);
            cells["B4"].PutValue(7);

            cells["C1"].PutValue("Q1");
            cells["C2"].PutValue("Q2");
            cells["C3"].PutValue("Y1");
            cells["C4"].PutValue("Y2");

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // تعيين خصائص شريط الخطأ لكل سلسلة في المخطط
            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                Series series = chart.NSeries[i];
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5;
            }

            // احفظ المصنف
            workbook.Save("ErrorBarTypeExample.xlsx");
            workbook.Save("ErrorBarTypeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


