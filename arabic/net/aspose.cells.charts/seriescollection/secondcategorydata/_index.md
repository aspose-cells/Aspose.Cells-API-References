---
title: "SeriesCollection.SecondCategoryData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SeriesCollection. تحصل أو تعين نطاق قيم محور الفئة الثاني. يمكن أن يكون نطاق خلايا مثل d1e10 أو تسلسل قيم مثل 26810. يؤثر فقط عندما يتم رسم بعض السلاسل على المحور الثاني"
type: docs
url: /ar/net/aspose.cells.charts/seriescollection/secondcategorydata/
---
## SeriesCollection.SecondCategoryData property

يحصل أو يضبط نطاق قيم محور الفئة الثاني. يمكن أن يكون نطاق خلايا (مثل "d1:e10"), أو تسلسل قيم (مثل "{2,6,8,10}"). يؤثر فقط عندما يتم رسم بعض السلاسل على المحور الثاني.

```csharp
public string SecondCategoryData { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertySecondCategoryDataDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Primary Categories");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["A4"].PutValue("Cat3");
            
            worksheet.Cells["B1"].PutValue("Secondary Categories");
            worksheet.Cells["B2"].PutValue("SubCat1");
            worksheet.Cells["B3"].PutValue("SubCat2");
            worksheet.Cells["B4"].PutValue("SubCat3");
            
            worksheet.Cells["C1"].PutValue("Values");
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(20);
            worksheet.Cells["C4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين بيانات السلسلة
            chart.NSeries.Add("C2:C4", true);
            
            // تعيين بيانات الفئة الأساسية
            chart.NSeries.CategoryData = "A2:A4";
            
            // تعيين بيانات الفئة الثانوية
            chart.NSeries.SecondCategoryData = "B2:B4";

            // احفظ المصنف
            workbook.Save("SecondCategoryDataDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


