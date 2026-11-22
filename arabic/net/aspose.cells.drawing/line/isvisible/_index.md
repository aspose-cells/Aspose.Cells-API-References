---
title: "Line.IsVisible"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Line. تمثل ما إذا كان الخط مرئيًا"
type: docs
url: /ar/net/aspose.cells.drawing/line/isvisible/
---
## Line.IsVisible property

يمثل ما إذا كان الخط مرئيًا.

```csharp
public bool IsVisible { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LinePropertyIsVisibleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
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
            
            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // الوصول إلى خطوط الشبكة الرئيسية وضبط الرؤية
            chart.CategoryAxis.MajorGridLines.IsVisible = true;
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            // تحقق من الرؤية
            Console.WriteLine("Major Gridlines Visible: " + chart.CategoryAxis.MajorGridLines.IsVisible);
        }
    }
}
```

### انظر أيضًا

* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


