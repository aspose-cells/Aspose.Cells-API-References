---
title: "CommandButtonActiveXControl.Accelerator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CommandButtonActiveXControl. Obtiene y establece la tecla de acceso rápido para el control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/accelerator/
---
## CommandButtonActiveXControl.Accelerator property

Obtiene y establece la tecla de acceso rápido para el control.

```csharp
public char Accelerator { get; set; }
```

### Ejemplos

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

### Ver también

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


