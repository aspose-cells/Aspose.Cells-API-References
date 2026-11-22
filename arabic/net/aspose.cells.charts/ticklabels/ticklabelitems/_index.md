---
title: "TickLabels.TickLabelItems"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TickLabels. تحصل على تسميات العلامات المعروضة للمحور"
type: docs
url: /ar/net/aspose.cells.charts/ticklabels/ticklabelitems/
---
## TickLabels.TickLabelItems property

يحصل على تسميات العلامات المعروضة للمحور.

```csharp
public TickLabelItem[] TickLabelItems { get; }
```

### ملاحظات

متاح فقط بعد استدعاء طريقة [`Calculate`](../../chart/calculate/).

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyTickLabelItemsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // أضف مخطط عمودي
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // حساب المخطط
            chart.Calculate();

            // احصل على محور الفئة وتسميات علاماته
            Aspose.Cells.Charts.Axis axis = chart.CategoryAxis;
            Aspose.Cells.Charts.TickLabelItem[] tickLabelItems = axis.TickLabels.TickLabelItems;

            // إضافة أشكال لتحديد موضع كل تسمية علامة
            for (int i = 0; i < tickLabelItems.Length; i++)
            {
                Aspose.Cells.Charts.TickLabelItem item = tickLabelItems[i];
                
                // أضف مستطيلًا حول كل تسمية علامة
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle, 
                    PlacementType.Move,
                    item.X,
                    item.Y,
                    item.X + item.Width,
                    item.Y + item.Height);
                
                shape.Fill.SolidFill.Transparency = 1;
                shape.Line.SolidFill.Color = Color.Blue;
            }

            // احفظ المصنف
            workbook.Save("TickLabelItemsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TickLabelItem](../../ticklabelitem/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


