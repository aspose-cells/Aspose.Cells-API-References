---
title: "DataLabels.SeparatorType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DataLabels. تحصل أو تعيين نوع الفاصل المستخدم لتسميات البيانات على المخطط"
type: docs
url: /ar/net/aspose.cells.charts/datalabels/separatortype/
---
## DataLabels.SeparatorType property

يحصل على أو يضبط نوع الفاصل المستخدم لتسميات البيانات في المخطط.

```csharp
public DataLabelsSeparatorType SeparatorType { get; set; }
```

### ملاحظات

لتعيين فاصل مخصص، يرجى ضبط الخاصية `SeparatorType` إلى Custom ثم تحديد القيمة المتوقعة لـ [`SeparatorValue`](../separatorvalue/).

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertySeparatorTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تمكين تسميات البيانات
            chart.NSeries[0].DataLabels.ShowValue = true;
            chart.NSeries[0].DataLabels.ShowCategoryName = true;
            
            // ضبط نوع الفاصل
            chart.NSeries[0].DataLabels.SeparatorType = DataLabelsSeparatorType.Space;

            // احفظ المصنف
            workbook.Save("DataLabelsSeparatorTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [DataLabelsSeparatorType](../../datalabelsseparatortype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


