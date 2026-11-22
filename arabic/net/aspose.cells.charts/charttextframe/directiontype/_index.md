---
title: "ChartTextFrame.DirectionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartTextFrame. تحصل وتضبط اتجاه النص"
type: docs
url: /ar/net/aspose.cells.charts/charttextframe/directiontype/
---
## ChartTextFrame.DirectionType property

يحصل على اتجاه النص ويضبطه.

```csharp
public virtual ChartTextDirectionType DirectionType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyDirectionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            // إضافة ورقة عمل تُعيد فهرستها، ثم نحصل على ورقة العمل باستخدام الفهرس
            int sheetIndex = workbook.Worksheets.Add();
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Q3");

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "C1:C3";

            // الوصول إلى العنوان وتكوينه
            ChartTextFrame title = chart.Title;
            title.Text = "Sample Chart";
            
            // عرض خاصية DirectionType
            title.DirectionType = ChartTextDirectionType.Vertical;
            
            // احفظ المصنف
            workbook.Save("ChartTextDirectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ChartTextDirectionType](../../charttextdirectiontype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


