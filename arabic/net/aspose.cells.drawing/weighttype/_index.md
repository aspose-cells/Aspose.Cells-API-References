---
title: "تعداد WeightType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Drawing.WeightType. يعدد أنواع الوزن لحدود الصورة أو خط المخطط"
type: docs
url: /ar/net/aspose.cells.drawing/weighttype/
---
## WeightType enumeration

يسرد أنواع الوزن لإطار الصورة أو خط المخطط.

```csharp
public enum WeightType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| HairLine | `-1` | يمثل وزن الخط الرفيع. |
| MediumLine | `1` | يمثل وزن الخط المتوسط. |
| SingleLine | `0` | يمثل وزن الخط الفردي. |
| WideLine | `2` | يمثل وزن الخط العريض. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassWeightTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف مخططًا واحصل على مساحة المخطط الخاصة به
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];
            ChartArea chartArea = chart.ChartArea;
            
            // اضبط نوع وزن الحدود
            chartArea.Border.Weight = WeightType.WideLine;
            
            // تحقق من نوع الوزن
            Console.WriteLine("Chart Area Border Weight: " + chartArea.Border.Weight);
            
            // احفظ المصنف
            workbook.Save("WeightTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


