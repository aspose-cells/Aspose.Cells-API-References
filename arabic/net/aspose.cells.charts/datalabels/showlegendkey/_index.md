---
title: "DataLabels.ShowLegendKey"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataLabels. تمثل سلوك عرض مفتاح وسيلة الإيضاح لتسمية البيانات في المخطط المحدد. صحيح إذا كان مفتاح وسيلة الإيضاح لتسمية البيانات مرئيًا"
type: docs
url: /ar/net/aspose.cells.charts/datalabels/showlegendkey/
---
## DataLabels.ShowLegendKey property

يمثل سلوك عرض مفتاح وسيلة الإيضاح لتسمية البيانات في مخطط محدد. صحيح إذا كان مفتاح وسيلة الإيضاح لتسمية البيانات مرئيًا.

```csharp
public bool ShowLegendKey { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowLegendKeyDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // احصل على تسميات البيانات
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            
            // تعيين ShowLegendKey إلى صحيح
            dataLabels.ShowLegendKey = true;
            Console.WriteLine("ShowLegendKey set to: " + dataLabels.ShowLegendKey);

            // احفظ المصنف
            workbook.Save("DataLabelsShowLegendKeyDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


