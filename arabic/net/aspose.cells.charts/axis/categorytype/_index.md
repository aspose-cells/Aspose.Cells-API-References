---
title: "Axis.CategoryType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Axis. تمثل نوع محور الفئة"
type: docs
url: /ar/net/aspose.cells.charts/axis/categorytype/
---
## Axis.CategoryType property

يمثل نوع محور الفئة.

```csharp
public CategoryType CategoryType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyCategoryTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Cat " + (i - 1));
                sheet.Cells["B" + i].PutValue(i * 10);
            }

            // إضافة مخطط
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 2, 25, 11);
            Chart chart = sheet.Charts[chartIndex];
            
            // تعيين مصدر بيانات المخطط
            chart.NSeries.Add("=Sheet1!$A$1:$B$10", true);

            // عرض خاصية CategoryType
            chart.CategoryAxis.CategoryType = Aspose.Cells.Charts.CategoryType.AutomaticScale;
            Console.WriteLine("CategoryType set to AutomaticScale");

            // احفظ المصنف
            workbook.Save("AxisPropertyCategoryTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* enum [CategoryType](../../categorytype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


