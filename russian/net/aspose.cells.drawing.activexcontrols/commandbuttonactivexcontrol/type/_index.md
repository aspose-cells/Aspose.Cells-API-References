---
title: "CommandButtonActiveXControl.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "CommandButtonActiveXControl property. Получает тип ActiveX‑контрола"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/type/
---
## CommandButtonActiveXControl.Type property

Получает тип ActiveX‑элемента управления.

```csharp
public override ControlType Type { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CommandButtonActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать кнопку команды с полным списком параметров
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.CommandButton,
                0,  // topRow
                0,  // top
                0,  // leftColumn
                0,  // left
                100,  // width
                100  // height
            );
            var control = (CommandButtonActiveXControl)shape.ActiveXControl;

            control.Caption = "CommandButton1";
            control.PicturePosition = ControlPicturePositionType.AboveCenter;
            control.Accelerator = (char)0;
            control.TakeFocusOnClick = false;
            control.IsWordWrapped = false;
            control.IsEnabled = true;

            Console.WriteLine($"Control Type: {control.Type}");
            Console.WriteLine($"Is CommandButton type: {control.Type == ControlType.CommandButton}");

            workbook.Save("CommandButtonDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ControlType](../../controltype/)
* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


