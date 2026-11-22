---
title: "TickLabels.RotationAngle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TickLabels. تمثل زاوية دوران النص باتجاه عقارب الساعة"
type: docs
url: /ar/net/aspose.cells.charts/ticklabels/rotationangle/
---
## TickLabels.RotationAngle property

يمثل زاوية دوران النص باتجاه عقارب الساعة.

```csharp
public int RotationAngle { get; set; }
```

### ملاحظات

0: غير مُدوَّر.255: من الأعلى إلى الأسفل.-90: للأسفل.90: للأعلى.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyRotationAngleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Category 1");
            sheet.Cells["A2"].PutValue("Category 2");
            sheet.Cells["A3"].PutValue("Category 3");
            sheet.Cells["B1"].PutValue(100);
            sheet.Cells["B2"].PutValue(200);
            sheet.Cells["B3"].PutValue(300);

            // إضافة مخطط
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // دوران تسميات العلامات على محور الفئة بزاوية 45 درجة
            chart.CategoryAxis.TickLabels.RotationAngle = 45;

            // احفظ المصنف
            workbook.Save("TickLabelsRotationDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


