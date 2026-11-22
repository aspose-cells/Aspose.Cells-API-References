---
title: "ToggleButtonActiveXControl.Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ToggleButtonActiveXControl. تشير إلى ما إذا كان العنصر محددًا أم لا"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/value/
---
## ToggleButtonActiveXControl.Value property

يشير إلى ما إذا كان التحكم محددًا أم لا.

```csharp
public CheckValueType Value { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر ToggleButton ActiveX control
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 1, 100, 30);
            ToggleButtonActiveXControl toggleButton = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // عيّن القيمة الأولية إلى غير محدد
            toggleButton.Value = CheckValueType.UnChecked;

            // تحقق وبدّل القيمة إذا كانت غير محددة
            if (toggleButton.Value == CheckValueType.UnChecked)
            {
                toggleButton.Value = CheckValueType.Checked;
            }

            // احفظ المصنف
            workbook.Save("ToggleButtonDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [CheckValueType](../../../aspose.cells.drawing/checkvaluetype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


