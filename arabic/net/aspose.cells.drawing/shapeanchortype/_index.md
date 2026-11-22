---
title: "التعداد ShapeAnchorType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.ShapeAnchorType enum. يمثل نوع التثبيت"
type: docs
url: /ar/net/aspose.cells.drawing/shapeanchortype/
---
## ShapeAnchorType enumeration

يمثل نوع المرساة.

```csharp
public enum ShapeAnchorType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| TwoCellAnchor | `0` | يمثل عنصرًا نائبًا لتثبيت خلية مزدوجة |
| OneCellAnchor | `1` | يمثل عنصرًا نائبًا لتثبيت خلية واحدة |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapeAnchorTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل صندوق مجموعة
            Shape box = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 300, 250);
            box.Text = "Sample Group Box";
            
            // وضح استخدام ShapeAnchorType
            box.AnchorType = ShapeAnchorType.TwoCellAnchor;
            box.UpperLeftRow = 2;
            box.UpperLeftColumn = 1;
            box.LowerRightRow = 8;
            box.LowerRightColumn = 4;

            // احفظ المصنف
            workbook.Save("ShapeAnchorTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


