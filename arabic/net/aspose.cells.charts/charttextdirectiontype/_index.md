---
title: "تعداد ChartTextDirectionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Charts.ChartTextDirectionType enum. يمثل نوع اتجاه النص للمخطط"
type: docs
url: /ar/net/aspose.cells.charts/charttextdirectiontype/
---
## ChartTextDirectionType enumeration

يمثل نوع اتجاه النص في المخطط.

```csharp
public enum ChartTextDirectionType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Horizontal | `0` | نوع الاتجاه الأفقي. |
| Vertical | `1` | نوع الاتجاه الرأسي. |
| Rotate90 | `2` | تدوير بزاوية تسعين درجة. |
| Rotate270 | `3` | تدوير بزاوية 270 درجة. |
| Stacked | `4` | نص مكدس. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartTextDirectionTypeDemo
    {
        public static void ChartTextDirectionTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة سلسلة بيانات إلى المخطط.
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // تحديد عنوان المخطط
            chart.Title.Text = "Sample Chart";
            chart.Title.Font.Color = Color.Blue;
            
            // تعيين اتجاه النص لعنوان المخطط.
            chart.Title.DirectionType = ChartTextDirectionType.Rotate90;
            
            // تعيين اتجاه النص لعنوان محور الفئة.
            chart.CategoryAxis.Title.Text = "Categories";
            chart.CategoryAxis.Title.DirectionType = ChartTextDirectionType.Vertical;
            
            // تعيين اتجاه النص لعنوان محور القيم.
            chart.ValueAxis.Title.Text = "Values";
            chart.ValueAxis.Title.DirectionType = ChartTextDirectionType.Horizontal;
            
            // احفظ المصنف
            workbook.Save("ChartTextDirectionTypeExample.xlsx");
            workbook.Save("ChartTextDirectionTypeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


