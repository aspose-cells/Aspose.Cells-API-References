---
title: "SeriesCollection.CategoryData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SeriesCollection. تحصل أو تعين نطاق قيم محور الفئة. يمكن أن يكون نطاق خلايا مثل d1e10 أو تسلسل قيم مثل 26810"
type: docs
url: /ar/net/aspose.cells.charts/seriescollection/categorydata/
---
## SeriesCollection.CategoryData property

يحصل أو يضبط نطاق قيم محور الفئة. يمكن أن يكون نطاق خلايا (مثل "d1:e10") أو تسلسل قيم (مثل "{2,6,8,10}").

```csharp
public string CategoryData { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertyCategoryDataDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Cat " + (i - 1));
                worksheet.Cells["B" + i].PutValue(i * 10);
            }
            
            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("=Sheet1!$B$2:$B$10", true);
            chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$10";
            
            // احفظ المصنف
            workbook.Save("CategoryDataDemo.xlsx");
            
            // تحقق من خاصية CategoryData
            Console.WriteLine("Chart CategoryData: " + chart.NSeries.CategoryData);
        }
    }
}
```

### انظر أيضًا

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


