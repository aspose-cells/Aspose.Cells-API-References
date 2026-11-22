---
title: "ChartTextFrame.IsAutomaticRotation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartTextFrame. تشير إلى ما إذا كان نص المخطط يتم تدويره تلقائيًا"
type: docs
url: /ar/net/aspose.cells.charts/charttextframe/isautomaticrotation/
---
## ChartTextFrame.IsAutomaticRotation property

يشير إلى ما إذا كان نص المخطط يتم تدويره تلقائيًا.

```csharp
public bool IsAutomaticRotation { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsAutomaticRotationDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى عنوان محور القيم وإظهار IsAutomaticRotation
            chart.ValueAxis.Title.Text = "Values";
            bool isAutoRotate = chart.ValueAxis.Title.IsAutomaticRotation;
            Console.WriteLine($"IsAutomaticRotation: {isAutoRotate}");

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


