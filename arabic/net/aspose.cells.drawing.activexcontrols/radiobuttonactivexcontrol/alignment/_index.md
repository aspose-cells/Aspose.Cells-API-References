---
title: "RadioButtonActiveXControl.Alignment"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية RadioButtonActiveXControl. يسترجع ويضبط موضع التسمية بالنسبة للعنصر"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/alignment/
---
## RadioButtonActiveXControl.Alignment property

يسترجع ويضبط موضع Caption بالنسبة للعنصر.

```csharp
public ControlCaptionAlignmentType Alignment { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class RadioButtonActiveXControlPropertyAlignmentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء مجموعة أشكال جديدة وإضافة عنصر ActiveX
            ShapeCollection shapes = worksheet.Shapes;
            Shape shape = shapes.AddActiveXControl(ControlType.RadioButton, 1, 1, 100, 30, 0, 0);
            RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape.ActiveXControl;
            
            // تعيين خاصية Alignment
            radioButton.Alignment = ControlCaptionAlignmentType.Left;
            
            // احفظ المصنف
            workbook.Save("RadioButtonAlignmentDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ControlCaptionAlignmentType](../../controlcaptionalignmenttype/)
* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


