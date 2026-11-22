---
title: "ToggleButtonActiveXControl.PicturePosition"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ToggleButtonActiveXControl. تحصل وتضبط موقع صورة العنصر بالنسبة لتسميته"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/pictureposition/
---
## ToggleButtonActiveXControl.PicturePosition property

يحصل على موقع صورة التحكم بالنسبة إلى التسمية التوضيحية الخاصة به ويضبطه.

```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertyPicturePositionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر تحكم ToggleButton ActiveX مع جميع المعلمات المطلوبة
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 100, 30, 0);
            var control = shape.ActiveXControl;

            if (control is ToggleButtonActiveXControl toggleButton)
            {
                // اضبط خاصية PicturePosition
                toggleButton.PicturePosition = ControlPicturePositionType.AboveLeft;

                // اضبط خصائص أخرى لتوضيح الوظيفة
                toggleButton.Caption = "Toggle Button";
                toggleButton.Picture = new byte[0]; // Empty picture for demo
            }

            // احفظ المصنف
            workbook.Save("ToggleButtonActiveXControlDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


