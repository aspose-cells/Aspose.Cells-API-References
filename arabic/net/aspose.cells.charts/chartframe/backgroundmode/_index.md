---
title: "ChartFrame.BackgroundMode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartFrame. تحصل وتضبط وضع عرض الخلفية. هذه الخاصية صالحة فقط في Excel 2003 أو الإصدارات الأقدم."
type: docs
url: /ar/net/aspose.cells.charts/chartframe/backgroundmode/
---
## ChartFrame.BackgroundMode property

تحصل وتضبط وضع عرض الخلفية. هذه الخاصية صالحة فقط في Excel 2003 أو الإصدارات الأقدم.

```csharp
[Obsolete("Use ChartFrame.Area.FillFormat.FillType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode BackgroundMode { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خاصية ChartFrame.Area.FillFormat.FillType. على سبيل المثال، إذا كنت بحاجة إلى تعيين BackgroundMode إلى Opaque، يمكنك استخدام الشيفرة التالية: Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ فبراير 2026. Aspose يعتذر عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyBackgroundModeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["B4"].PutValue(20);

            // إضافة مخطط
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // تعيين بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // عرض خاصية BackgroundMode
            chart.ChartArea.BackgroundMode = Aspose.Cells.Charts.BackgroundMode.Transparent;
            chart.PlotArea.BackgroundMode = Aspose.Cells.Charts.BackgroundMode.Automatic;

            // احفظ المصنف
            workbook.Save("ChartBackgroundModeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [BackgroundMode](../../backgroundmode/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


