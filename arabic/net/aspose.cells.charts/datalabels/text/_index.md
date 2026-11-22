---
title: "DataLabels.Text"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataLabels. تحصل أو تعيين نص تسمية البيانات"
type: docs
url: /ar/net/aspose.cells.charts/datalabels/text/
---
## DataLabels.Text property

يحصل على أو يضبط نص تسمية البيانات.

```csharp
public override string Text { get; set; }
```

### ملاحظات

يعمل فقط عندما تكون هذه تسمية بيانات لنقطة مخطط.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyTextDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["A4"].PutValue("Product C");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تمكين تسميات البيانات
            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                Aspose.Cells.Charts.Series series = chart.NSeries[i];
                series.DataLabels.ShowValue = true;
                
                // تخصيص نص تسمية البيانات
                for (int j = 0; j < series.Points.Count; j++)
                {
                    series.Points[j].DataLabels.Text = $"+{series.Points[j].YValue}";
                }
            }

            // احفظ المصنف
            workbook.Save("DataLabelsTextDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


