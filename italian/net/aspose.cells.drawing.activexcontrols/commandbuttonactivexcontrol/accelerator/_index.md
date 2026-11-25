---
title: "CommandButtonActiveXControl.Accelerator"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "CommandButtonActiveXControl property. Ottiene e imposta il tasto di accelerazione per il controllo"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/accelerator/
---
## CommandButtonActiveXControl.Accelerator property

Ottiene e imposta il tasto di accelerazione per il controllo.

```csharp
public char Accelerator { get; set; }
```

### Esempi

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

### Vedi anche

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


