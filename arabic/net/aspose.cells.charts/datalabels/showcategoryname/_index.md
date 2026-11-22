---
title: "DataLabels.ShowCategoryName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataLabels. تمثل سلوك عرض اسم الفئة لتسمية البيانات في المخطط المحدد. صحيحة لعرض اسم الفئة لتسميات البيانات على المخطط. خاطئة للإخفاء."
type: docs
url: /ar/net/aspose.cells.charts/datalabels/showcategoryname/
---
## DataLabels.ShowCategoryName property

يمثل سلوك عرض اسم الفئة لتسمية البيانات في مخطط محدد. صحيح لعرض اسم الفئة لتسميات البيانات في المخطط. خطأ لإخفائه.

```csharp
public bool ShowCategoryName { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowCategoryNameDemo
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

            // أضف مخطط عمودي
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تمكين تسميات البيانات وضبط الخصائص
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.ShowCategoryName = true;
            dataLabels.SeparatorType = DataLabelsSeparatorType.Semicolon;

            // احفظ المصنف
            workbook.Save("DataLabelsShowCategoryNameDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


