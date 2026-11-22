---
title: "تعداد DataLabelsSeparatorType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Charts.DataLabelsSeparatorType. يمثل نوع الفاصل لملصقات البيانات"
type: docs
url: /ar/net/aspose.cells.charts/datalabelsseparatortype/
---
## DataLabelsSeparatorType enumeration

يمثل نوع الفاصل لتسميات البيانات.

```csharp
public enum DataLabelsSeparatorType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Auto | `0` | يمثل الفاصل التلقائي |
| Space | `1` | يمثل مسافة(\" \") |
| Comma | `2` | يمثل فاصلة(\",\") |
| Semicolon | `3` | يمثل فاصلة منقوطة(\";\") |
| Period | `4` | يمثل نقطة(\".\") |
| NewLine | `5` | يمثل سطرًا جديدًا(\"\\n\") |
| Custom | `6` | يمثل فاصلًا مخصصًا |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class DataLabelsSeparatorTypeDemo
    {
        public static void DataLabelsSeparatorTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات للمخطط
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // أضف سلسلة البيانات إلى المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى ملصقات البيانات للسلسلة الأولى
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // عيّن نوع الفاصل إلى الفاصلة
            dataLabels.SeparatorType = DataLabelsSeparatorType.Comma;

            // فعّل تسميات البيانات واضبط بعض الخصائص
            dataLabels.ShowCategoryName = true;
            dataLabels.ShowValue = true;
            dataLabels.Position = LabelPositionType.InsideBase;

            // عيّن خصائص الخط
            dataLabels.Font.Color = Color.Blue;
            dataLabels.Font.IsBold = true;

            // احفظ المصنف
            workbook.Save("DataLabelsSeparatorTypeExample.xlsx");
            workbook.Save("DataLabelsSeparatorTypeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


