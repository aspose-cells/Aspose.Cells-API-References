---
title: "Shape.HtmlText"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الشكل. تحصل وتعيّن سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذا مربع النص"
type: docs
url: /ar/net/aspose.cells.drawing/shape/htmltext/
---
## Shape.HtmlText property

يحصل ويضبط سلسلة HTML التي تحتوي على البيانات وبعض الصيغ في مربع النص هذا.

```csharp
public string HtmlText { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyHtmlTextDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // تحقق مما إذا كان HtmlText فارغًا وقم بتعيينه إذا لزم الأمر
            string html = shape.HtmlText;
            if (string.IsNullOrEmpty(html))
            {
                shape.HtmlText = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>";
            }

            // احفظ المصنف
            workbook.Save("ShapeHtmlTextDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


