---
title: "ChartFrame.IsInnerMode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartFrame. تشير إلى ما إذا كان حجم مساحة الرسم يتضمن علامات الفواصل وتسميات المحاور. القيمة False تعني أن الحجم سيحدد حجم مساحة الرسم وعلامات الفواصل وتسميات المحاور"
type: docs
url: /ar/net/aspose.cells.charts/chartframe/isinnermode/
---
## ChartFrame.IsInnerMode property

يشير إلى ما إذا كان حجم مساحة الرسم يتضمن علامات الفواصل وعناوين المحاور. القيمة False تعني أن الحجم سيحدد حجم مساحة الرسم وعلامات الفواصل وعناوين المحاور.

```csharp
public bool IsInnerMode { get; set; }
```

### ملاحظات

فقط لملف Xlsx.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyIsInnerModeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى إطار المخطط وعرض IsInnerMode
            Aspose.Cells.Charts.ChartFrame chartFrame = chart.ChartArea;
            chartFrame.IsInnerMode = true; // Set to use inner mode
            
            // ضبط بعض الخصائص الأساسية لإظهار التأثير
            chartFrame.Border.Color = Color.Blue;
            chartFrame.Border.Style = Aspose.Cells.Drawing.LineType.Solid;
            chartFrame.Area.ForegroundColor = Color.LightYellow;

            workbook.Save("ChartFrameIsInnerModeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


