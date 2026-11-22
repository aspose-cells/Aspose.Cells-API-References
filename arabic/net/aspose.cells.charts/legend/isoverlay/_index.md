---
title: "Legend.IsOverLay"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Legend. يحصل أو يضبط ما إذا كان عرض legend دون تداخل مع المخطط"
type: docs
url: /ar/net/aspose.cells.charts/legend/isoverlay/
---
## Legend.IsOverLay property

يحصل أو يضبط ما إذا كان يتم عرض وسيلة الإيضاح دون تداخلها مع المخطط.

```csharp
public bool IsOverLay { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendPropertyIsOverLayDemo
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
            
            // اضبط تراكب legend
            chart.Legend.IsOverLay = true;
            
            // احفظ المصنف
            workbook.Save("LegendOverlayDemo.xlsx");
            
            Console.WriteLine("Chart with overlay legend created successfully.");
        }
    }
}
```

### انظر أيضًا

* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


