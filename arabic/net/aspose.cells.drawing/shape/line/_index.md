---
title: "Shape.Line"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Shape. تحصل على نمط الخط"
type: docs
url: /ar/net/aspose.cells.drawing/shape/line/
---
## Shape.Line property

يحصل على نمط الخط

```csharp
public LineFormat Line { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLineDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل خط (يرجع LineShape مباشرةً)
            LineShape lineShape = worksheet.Shapes.AddLine(1, 0, 1, 0, 5, 100);

            // الوصول إلى خصائص الخط وتعديلها
            LineFormat lineFormat = lineShape.Line;
            lineFormat.CompoundType = MsoLineStyle.ThickThin;
            lineFormat.DashStyle = MsoLineDashStyle.DashDot;
            lineFormat.Weight = 3.0;
            lineFormat.BeginArrowheadStyle = MsoArrowheadStyle.Arrow;
            lineFormat.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // احفظ المصنف
            workbook.Save("LineShapeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [LineFormat](../../lineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


