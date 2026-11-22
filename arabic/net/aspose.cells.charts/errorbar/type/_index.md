---
title: "ErrorBar.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ErrorBar. تمثل نوع مقدار شريط الخطأ"
type: docs
url: /ar/net/aspose.cells.charts/errorbar/type/
---
## ErrorBar.Type property

يمثل نوع مقدار شريط الخطأ.

```csharp
public ErrorBarType Type { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // أضف بيانات تجريبية
            ws.Cells["A1"].PutValue(5);
            ws.Cells["A2"].PutValue(3);
            
            // إنشاء مخطط
            int chartIndex = ws.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = ws.Charts[chartIndex];
            
            // إضافة بيانات السلسلة
            chart.NSeries.Add("A3:A10", true);
            Series series = chart.NSeries[0];
            
            // اضبط نوع شريط الخطأ المخصص والقيم
            series.YErrorBar.Type = ErrorBarType.Custom;
            series.YErrorBar.PlusValue = "=Sheet1!A1";
            series.YErrorBar.MinusValue = "=Sheet1!A2";
            
            // احفظ المصنف
            wb.Save("ErrorBarDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ErrorBarType](../../errorbartype/)
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


