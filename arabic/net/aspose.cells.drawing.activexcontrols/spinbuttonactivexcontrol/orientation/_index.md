---
title: "SpinButtonActiveXControl.Orientation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "SpinButtonActiveXControl خاصية. يحصل ويضبط ما إذا كان SpinButton أو ScrollBar موجهًا عموديًا أو أفقيًا"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/orientation/
---
## SpinButtonActiveXControl.Orientation property

يحصل على ويضبط ما إذا كان SpinButton أو ScrollBar موجهًا عمودياً أو أفقياً.

```csharp
public ControlScrollOrientation Orientation { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyOrientationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر SpinButton ActiveX control
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 1, 1, 100, 50, 100, 50);
            SpinButtonActiveXControl spinButton = (SpinButtonActiveXControl)shape.ActiveXControl;

            // تحقق وعدل الاتجاه
            if (spinButton.Orientation == ControlScrollOrientation.Auto)
            {
                spinButton.Orientation = ControlScrollOrientation.Horizontal;
            }

            // احفظ المصنف
            workbook.Save("SpinButtonOrientationDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ControlScrollOrientation](../../controlscrollorientation/)
* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


