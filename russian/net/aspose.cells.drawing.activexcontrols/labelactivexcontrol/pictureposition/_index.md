---
title: "LabelActiveXControl.PicturePosition"
second_title: "Справочник API Aspose.Cells для .NET"
description: "LabelActiveXControl property. Получает и задает расположение изображения элемента управления относительно его подписи"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/pictureposition/
---
## LabelActiveXControl.PicturePosition property

Получает и задает расположение изображения элемента управления относительно его подписи.

```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```

### Примеры

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

### См. также

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


