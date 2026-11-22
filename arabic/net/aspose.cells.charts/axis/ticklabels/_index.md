---
title: "Axis.TickLabels"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Axis. تُرجع كائن TickLabels يمثل تسميات علامات التحديد للمحور المحدد"
type: docs
url: /ar/net/aspose.cells.charts/axis/ticklabels/
---
## Axis.TickLabels property

يرجع كائن `TickLabels` يمثل تسميات علامات التحديد للمحور المحدد.

```csharp
public TickLabels TickLabels { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTickLabelsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // الوصول إلى تسميات علامات محور الفئة
            Aspose.Cells.Charts.Axis axis = chart.CategoryAxis;
            axis.TickLabels.Font.IsBold = true;
            axis.TickLabels.Font.Color = System.Drawing.Color.Red;
            axis.TickLabels.RotationAngle = 45;
            
            // احفظ المصنف
            workbook.Save("AxisPropertyTickLabelsDemo_out.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [TickLabels](../../ticklabels/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


