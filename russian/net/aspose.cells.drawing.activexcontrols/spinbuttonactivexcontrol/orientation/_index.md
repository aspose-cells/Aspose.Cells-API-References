---
title: "SpinButtonActiveXControl.Orientation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "SpinButtonActiveXControl property. Получает и задает, ориентирован ли SpinButton или ScrollBar вертикально или горизонтально"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/orientation/
---
## SpinButtonActiveXControl.Orientation property

Получает и задает, ориентированы ли SpinButton или ScrollBar вертикально или горизонтально.

```csharp
public ControlScrollOrientation Orientation { get; set; }
```

### Примеры

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

            // Добавьте SpinButton ActiveX control
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 1, 1, 100, 50, 100, 50);
            SpinButtonActiveXControl spinButton = (SpinButtonActiveXControl)shape.ActiveXControl;

            // Проверьте и измените ориентацию
            if (spinButton.Orientation == ControlScrollOrientation.Auto)
            {
                spinButton.Orientation = ControlScrollOrientation.Horizontal;
            }

            // Сохраните книгу
            workbook.Save("SpinButtonOrientationDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ControlScrollOrientation](../../controlscrollorientation/)
* class [SpinButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


