---
title: "DataLabels.SeparatorValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataLabels. يحصل على أو يضبط قيمة الفاصل المستخدمة لتسميات البيانات في المخطط"
type: docs
url: /ar/net/aspose.cells.charts/datalabels/separatorvalue/
---
## DataLabels.SeparatorValue property

يحصل على أو يضبط قيمة الفاصل المستخدمة لتسميات البيانات في المخطط.

```csharp
public string SeparatorValue { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertySeparatorValueDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تكوين DataLabels
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.ShowCategoryName = true;
            dataLabels.SeparatorValue = " | "; // Demonstrate SeparatorValue property
            dataLabels.Position = LabelPositionType.Center;

            workbook.Save("DataLabelsSeparatorValueDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


