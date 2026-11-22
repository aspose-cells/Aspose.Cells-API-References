---
title: "SeriesCollection.IsColorVaried"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SeriesCollection. تمثل ما إذا كان لون النقاط متنوعًا"
type: docs
url: /ar/net/aspose.cells.charts/seriescollection/iscolorvaried/
---
## SeriesCollection.IsColorVaried property

يمثل ما إذا كان لون النقاط متنوعًا.

```csharp
public bool IsColorVaried { get; set; }
```

### ملاحظات

يعمل فقط مع مخطط دائري أو عندما تكون هناك سلسلة واحدة فقط.

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertyIsColorVariedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // بيانات عينة
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Region");
            cells["A2"].PutValue("France");
            cells["A3"].PutValue("Germany");
            cells["A4"].PutValue("England");
            cells["A5"].PutValue("USA");
            cells["B1"].PutValue("Sales");
            cells["B2"].PutValue(70000);
            cells["B3"].PutValue(55000);
            cells["B4"].PutValue(30000);
            cells["B5"].PutValue(85000);

            // إنشاء مخطط
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            
            // إضافة سلسلة
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // تعيين خاصية IsColorVaried
            chart.NSeries.IsColorVaried = true;
            
            // احفظ المصنف
            workbook.Save("SeriesCollectionPropertyIsColorVariedDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


