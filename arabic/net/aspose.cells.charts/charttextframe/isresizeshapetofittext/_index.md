---
title: "ChartTextFrame.IsResizeShapeToFitText"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartTextFrame. تحصل أو تعيين ما إذا كان يجب أن يتم تعديل حجم الشكل تلقائيًا لاحتواء النص الموصوف بداخله بالكامل. تعديل الحجم التلقائي هو عندما يتم تحجيم النص داخل الشكل لاحتواء جميع النص داخل."
type: docs
url: /ar/net/aspose.cells.charts/charttextframe/isresizeshapetofittext/
---
## ChartTextFrame.IsResizeShapeToFitText property

يحصل أو يحدد ما إذا كان يجب أن يتناسب الشكل تلقائيًا لاحتواء النص الموصوف بداخله بالكامل. التناسب التلقائي هو عندما يتم تحجيم النص داخل الشكل لتضمين كل النص داخل.

```csharp
public bool IsResizeShapeToFitText { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsResizeShapeToFitTextDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // أضف مخطط عمودي
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين بيانات السلسلة
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // الوصول إلى تسميات البيانات
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.Position = LabelPositionType.Center;

            // إظهار خاصية IsResizeShapeToFitText
            foreach (ChartPoint point in chart.NSeries[0].Points)
            {
                // تعطيل تعديل حجم الشكل تلقائيًا ليتناسب مع النص
                point.DataLabels.IsResizeShapeToFitText = false;
                
                // تعيين عرض مخصص أصغر مما يتطلبه النص عادةً
                point.DataLabels.Width = 50;
            }

            // احفظ المصنف
            workbook.Save("ChartTextFramePropertyIsResizeShapeToFitTextDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


