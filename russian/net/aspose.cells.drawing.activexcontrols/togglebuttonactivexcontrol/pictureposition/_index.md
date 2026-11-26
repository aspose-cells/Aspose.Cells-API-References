---
title: "ToggleButtonActiveXControl.PicturePosition"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ToggleButtonActiveXControl. Получает и задает расположение изображения элемента управления относительно его подписи"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/pictureposition/
---
## ToggleButtonActiveXControl.PicturePosition property

Получает и задает расположение изображения элемента управления относительно его подписи.

```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```

### Примеры

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

            // Добавьте элемент управления ToggleButton ActiveX со всеми необходимыми параметрами
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 100, 30, 0);
            var control = shape.ActiveXControl;

            if (control is ToggleButtonActiveXControl toggleButton)
            {
                // Установите свойство PicturePosition
                toggleButton.PicturePosition = ControlPicturePositionType.AboveLeft;

                // Установите другие свойства для демонстрации функциональности
                toggleButton.Caption = "Toggle Button";
                toggleButton.Picture = new byte[0]; // Empty picture for demo
            }

            // Сохраните книгу
            workbook.Save("ToggleButtonActiveXControlDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


