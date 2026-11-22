---
title: "ChartFrame.IsDefaultPosBeSet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartFrame. تشير إلى ما إذا تم تعيين الموضع الافتراضي DefaultX DefaultY DefaultWidth و DefaultHeight"
type: docs
url: /ar/net/aspose.cells.charts/chartframe/isdefaultposbeset/
---
## ChartFrame.IsDefaultPosBeSet property

يشير إلى ما إذا تم تعيين الموقع الافتراضي (DefaultX, DefaultY, DefaultWidth و DefaultHeight).

```csharp
public bool IsDefaultPosBeSet { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyIsDefaultPosBeSetDemo
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

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Bar, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى تسميات البيانات
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            
            // إظهار خاصية IsDefaultPosBeSet
            Console.WriteLine("IsDefaultPosBeSet before setting position: " + dataLabels.IsDefaultPosBeSet);
            
            // غيّر الموضع وتحقق من الخاصية مرة أخرى
            dataLabels.Position = LabelPositionType.InsideBase;
            Console.WriteLine("IsDefaultPosBeSet after setting position: " + dataLabels.IsDefaultPosBeSet);
        }
    }
}
```

### انظر أيضًا

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


