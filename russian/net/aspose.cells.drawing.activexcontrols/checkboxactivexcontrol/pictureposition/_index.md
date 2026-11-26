---
title: "CheckBoxActiveXControl.PicturePosition"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CheckBoxActiveXControl. Получает и задает расположение изображения элемента управления относительно его подписи"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/pictureposition/
---
## CheckBoxActiveXControl.PicturePosition property

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
    public class CheckBoxActiveXControlPropertyPicturePositionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте элемент управления CheckBox ActiveX со всеми необходимыми параметрами
            var shape = worksheet.Shapes.AddActiveXControl(
                ControlType.CheckBox, 
                10,  // left
                10,  // top
                150, // width
                30,  // height
                0,   // leftOffset
                0    // topOffset
            );
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Настройте свойства CheckBox
            checkBox.Caption = "Sample CheckBox";
            checkBox.PicturePosition = ControlPicturePositionType.Center;
            checkBox.IsAutoSize = true;

            // Сохраните книгу
            workbook.Save("CheckBoxPicturePositionDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


