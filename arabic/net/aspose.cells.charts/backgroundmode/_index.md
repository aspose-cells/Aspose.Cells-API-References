---
title: "Enum BackgroundMode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Charts.BackgroundMode. يمثل وضع عرض الخلفية"
type: docs
url: /ar/net/aspose.cells.charts/backgroundmode/
---
## BackgroundMode enumeration

يمثل وضع عرض الخلفية.

```csharp
public enum BackgroundMode
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Automatic | `0` | تلقائي |
| Opaque | `1` | معتم |
| Transparent | `2` | شفاف |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class BackgroundModeDemo
    {
        public static void BackgroundModeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // احصل على مرجع ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض البيانات النموذجية إلى الخلايا
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // أضف NSeries (مصدر بيانات المخطط) إلى المخطط من الخلية \"A1\" إلى \"B3\"
            chart.NSeries.Add("A1:B3", true);
            
            // الوصول إلى منطقة المخطط
            ChartArea chartArea = chart.ChartArea;

            // حدد لون المقدمة لمنطقة المخطط
            chartArea.Area.ForegroundColor = Color.Yellow;

            // حدد وضع الخلفية لمنطقة المخطط
            chartArea.BackgroundMode = BackgroundMode.Opaque;
            chartArea.Area.Transparency = 0.8;           
            
            
            // حدد ظل منطقة المخطط
            chartArea.Shadow = true;
            
            // احفظ المصنف
            workbook.Save("BackgroundModeExample.xlsx");
            workbook.Save("BackgroundModeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


