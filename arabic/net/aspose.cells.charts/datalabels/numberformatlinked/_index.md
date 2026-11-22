---
title: "DataLabels.NumberFormatLinked"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataLabels. صحيحة إذا كان تنسيق الأرقام مرتبطًا بالخلايا بحيث يتغير تنسيق الأرقام في التسميات عندما يتغير في الخلايا"
type: docs
url: /ar/net/aspose.cells.charts/datalabels/numberformatlinked/
---
## DataLabels.NumberFormatLinked property

صحيح إذا كان تنسيق الرقم مرتبطًا بالخلايا (بحيث يتغير تنسيق الرقم في التسميات عندما يتغير في الخلايا).

```csharp
public bool NumberFormatLinked { get; set; }
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
    public class DataLabelsPropertyNumberFormatLinkedDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["C1"].PutValue("Formatted Value");
            worksheet.Cells["C2"].PutValue("100 units");
            worksheet.Cells["C3"].PutValue("200 units");

            // إنشاء مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة سلسلة
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // تكوين تسميات البيانات
            var series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            series.DataLabels.LinkedSource = "C2:C3";
            series.DataLabels.NumberFormatLinked = true; // Link number format from source cells
            
            // احفظ المصنف
            workbook.Save("DataLabelsNumberFormatLinkedDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


