---
title: "LabelActiveXControl.PicturePosition"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LabelActiveXControl. يحصل ويضبط موقع صورة العنصر بالنسبة إلى التسمية التوضيحية"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/pictureposition/
---
## LabelActiveXControl.PicturePosition property

يحصل على موقع صورة التحكم بالنسبة إلى التسمية التوضيحية الخاصة به ويضبطه.

```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyPicturePositionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 5, 0, 1, 1, 100, 20);
            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            label.Caption = "Demo Label";
            label.PicturePosition = ControlPicturePositionType.AboveLeft;
            
            Console.WriteLine("Label Picture Position: " + label.PicturePosition);
            
            workbook.Save("LabelActiveXControlPicturePositionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


