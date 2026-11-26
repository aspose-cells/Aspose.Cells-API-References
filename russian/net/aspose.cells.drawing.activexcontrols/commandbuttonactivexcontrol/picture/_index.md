---
title: "CommandButtonActiveXControl.Picture"
second_title: "Справочник API Aspose.Cells для .NET"
description: "CommandButtonActiveXControl property. Получает и задает данные изображения"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/picture/
---
## CommandButtonActiveXControl.Picture property

Получает и задает данные изображения.

```csharp
public byte[] Picture { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CommandButtonActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать форму для размещения элемента управления ActiveX со всеми необходимыми параметрами
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.CommandButton, 
                1,  // top row
                1,  // left column
                0,  // top position
                0,  // left position
                100, // width
                30); // height
                
            CommandButtonActiveXControl button = (CommandButtonActiveXControl)shape.ActiveXControl;

            // Установить свойства
            button.Caption = "Click Me";
            button.PicturePosition = ControlPicturePositionType.AboveCenter;

            // Задайте изображение (пустой массив байтов представляет отсутствие изображения)
            button.Picture = new byte[0];

            // Сохраните книгу
            workbook.Save("CommandButtonWithPicture.xlsx");

            // Проверьте свойство picture
            Console.WriteLine("Picture is null: " + (button.Picture == null));
        }
    }
}
```

### См. также

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


