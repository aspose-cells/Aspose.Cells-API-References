---
title: "SpinButtonActiveXControl.Position"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SpinButtonActiveXControl. تسترجع وتضبط القيمة"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/position/
---
## SpinButtonActiveXControl.Position property

يحصل على ويضبط القيمة.

```csharp
public int Position { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpinButtonActiveXControlPropertyPositionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر SpinButton ActiveX control
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.SpinButton,
                1, 0, 1, 0, 100, 30);

            // احصل على عنصر ActiveX واضبط خاصية Position
            var spinButton = (Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl)shape.ActiveXControl;
            spinButton.Position = 30;

            // احفظ المصنف
            workbook.Save("SpinButtonPositionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


