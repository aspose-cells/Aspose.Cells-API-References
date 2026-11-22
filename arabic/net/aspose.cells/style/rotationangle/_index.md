---
title: "Style.RotationAngle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تمثل زاوية دوران النص"
type: docs
url: /ar/net/aspose.cells/style/rotationangle/
---
## Style.RotationAngle property

يمثل زاوية دوران النص.

```csharp
public int RotationAngle { get; set; }
```

### ملاحظات

0: غير مُدوَّر.

255: من الأعلى إلى الأسفل.

-90: Downward.

90: للأعلى.

يمكنك تعيين 255 أو قيمة تتراوح بين -90 إلى 90.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyRotationAngleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نمط بزاويات دوران مختلفة
            Style style1 = workbook.CreateStyle();
            style1.RotationAngle = -90;
            worksheet.Cells["B2"].PutValue("Text rotated -90°");
            worksheet.Cells["B2"].SetStyle(style1);

            Style style2 = workbook.CreateStyle();
            style2.RotationAngle = 90;
            worksheet.Cells["C3"].PutValue("Text rotated 90°");
            worksheet.Cells["C3"].SetStyle(style2);

            Style style3 = workbook.CreateStyle();
            style3.RotationAngle = 255;
            worksheet.Cells["D4"].PutValue("Text rotated 255°");
            worksheet.Cells["D4"].SetStyle(style3);

            // احفظ المصنف
            workbook.Save("output_rotation_angles.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


