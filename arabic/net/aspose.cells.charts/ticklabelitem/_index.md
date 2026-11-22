---
title: "الفئة TickLabelItem"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Charts.TickLabelItem. تمثل تسمية علامة على المخطط"
type: docs
url: /ar/net/aspose.cells.charts/ticklabelitem/
---
## TickLabelItem class

يمثل تسمية علامة في المخطط.

```csharp
public class TickLabelItem
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Height](../../aspose.cells.charts/ticklabelitem/height/) { get; } | ارتفاع عنصر Ticklabel كنسبة من ارتفاع المخطط. |
| [Width](../../aspose.cells.charts/ticklabelitem/width/) { get; } | عرض عنصر Ticklabel كنسبة من عرض المخطط. |
| [X](../../aspose.cells.charts/ticklabelitem/x/) { get; } | إحداثيات س لعنصر Ticklabel كنسبة من عرض المخطط. |
| [Y](../../aspose.cells.charts/ticklabelitem/y/) { get; } | إحداثيات ص لعنصر Ticklabel كنسبة من ارتفاع المخطط. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartsClassTickLabelItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // أضف مخطط عمودي
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // حساب المخطط
            chart.Calculate();

            // الوصول إلى تسميات علامات محور الفئة
            Axis axis = chart.CategoryAxis;
            TickLabelItem[] tickLabelItems = axis.TickLabels.TickLabelItems;

            // إضافة أشكال لتحديد موضع كل تسمية علامة
            foreach (TickLabelItem item in tickLabelItems)
            {
                // إضافة مستطيل حول تسمية العلامة
                Shape rectangle = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle,
                    PlacementType.Move,
                    item.X,
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                rectangle.Fill.SolidFill.Transparency = 1;
                rectangle.Line.SolidFill.Color = Color.Blue;

                // إضافة دائرة بجوار تسمية العلامة
                Shape circle = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Oval,
                    PlacementType.Move,
                    item.X + item.Width,
                    item.Y,
                    item.X + item.Width + item.Height,
                    item.Y + item.Height);
                circle.Fill.SolidFill.Color = Color.Red;
            }

            // احفظ المصنف
            workbook.Save("TickLabelItemDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


