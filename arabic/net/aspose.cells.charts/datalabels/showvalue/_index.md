---
title: "DataLabels.ShowValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataLabels. تمثل سلوك عرض قيم تسميات البيانات لمخطط محدد. True يعرض القيم. False لإخفائها"
type: docs
url: /ar/net/aspose.cells.charts/datalabels/showvalue/
---
## DataLabels.ShowValue property

يمثل سلوك عرض قيم تسمية البيانات في مخطط محدد. صحيح يعرض القيم. خطأ يخفيها.

```csharp
public bool ShowValue { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowValueDemo
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

            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تمكين تسميات البيانات وعرض القيم
            chart.NSeries[0].DataLabels.ShowValue = true;
            chart.NSeries[0].DataLabels.Position = LabelPositionType.Center;

            // احفظ المصنف
            workbook.Save("DataLabelsShowValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


