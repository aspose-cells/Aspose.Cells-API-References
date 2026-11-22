---
title: "ChartTextFrame.LinkedSource"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ChartTextFrame. تحصل أو تعيين إشارة إلى ورقة العمل"
type: docs
url: /ar/net/aspose.cells.charts/charttextframe/linkedsource/
---
## ChartTextFrame.LinkedSource property

يحصل ويحدد مرجعًا إلى ورقة العمل.

```csharp
public virtual string LinkedSource { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyLinkedSourceDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["P1"].PutValue("Chart Title");
            
            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين عنوان المخطط وربطه بالخلية P1
            chart.Title.Text = "Linked Title";
            chart.Title.LinkedSource = "='" + worksheet.Name + "'!$P$1";
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            // تحقق من المصدر المرتبط
            Console.WriteLine("Chart Title Linked Source: " + chart.Title.LinkedSource);
        }
    }
}
```

### انظر أيضًا

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


