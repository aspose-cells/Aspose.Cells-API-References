---
title: "TextBoxActiveXControl.BorderStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextBoxActiveXControl. تحصل وتضبط نوع الحدود المستخدمة من قبل عنصر التحكم"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/borderstyle/
---
## TextBoxActiveXControl.BorderStyle property

يحصل ويضبط نوع الإطار المستخدم من قبل العنصر.

```csharp
public ControlBorderType BorderStyle { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyBorderStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر تحكم TextBox ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 1, 100, 100, 0);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;

            // اضبط خاصية BorderStyle
            textBox.BorderStyle = ControlBorderType.Single;

            // احفظ المصنف
            workbook.Save("TextBoxActiveXControlBorderStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ControlBorderType](../../controlbordertype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


