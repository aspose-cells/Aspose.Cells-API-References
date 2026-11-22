---
title: "PatternFill.Pattern"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PatternFill. تحصل أو تعين نوع نمط التعبئة"
type: docs
url: /ar/net/aspose.cells.drawing/patternfill/pattern/
---
## PatternFill.Pattern property

الحصول على أو تعيين نوع نمط الملء

```csharp
public FillPattern Pattern { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PatternFillPropertyPatternDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // تعيين نمط التعبئة للسلسلة الأولى
            chart.NSeries[0].Area.FillFormat.FillType = FillType.Pattern;
            chart.NSeries[0].Area.FillFormat.PatternFill.Pattern = FillPattern.WideDownwardDiagonal;
            
            // احفظ المصنف
            workbook.Save("PatternFillDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [FillPattern](../../fillpattern/)
* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


