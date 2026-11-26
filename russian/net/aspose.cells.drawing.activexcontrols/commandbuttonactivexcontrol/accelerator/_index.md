---
title: "CommandButtonActiveXControl.Accelerator"
second_title: "Справочник API Aspose.Cells для .NET"
description: "CommandButtonActiveXControl property. Получает и задает клавишу-ускоритель для элемента управления"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/accelerator/
---
## CommandButtonActiveXControl.Accelerator property

Получает и задает клавишу ускорителя для элемента управления.

```csharp
public char Accelerator { get; set; }
```

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CommandButtonActiveXControlPropertyAcceleratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            Shape shape = sheet.Shapes.AddActiveXControl(ControlType.CommandButton, 0, 0, 0, 0, 30, 100);
            CommandButtonActiveXControl button = (CommandButtonActiveXControl)shape.ActiveXControl;

            button.Caption = "CommandButton1";
            button.Accelerator = 'A';
            button.PicturePosition = ControlPicturePositionType.AboveCenter;
            button.IsEnabled = true;

            workbook.Save("CommandButtonAcceleratorDemo.xlsx");
        }
    }
}
```

### См. также

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


