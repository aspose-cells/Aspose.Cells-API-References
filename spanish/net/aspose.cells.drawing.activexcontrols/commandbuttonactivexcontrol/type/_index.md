---
title: "CommandButtonActiveXControl.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CommandButtonActiveXControl. Obtiene el tipo del control ActiveX"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/type/
---
## CommandButtonActiveXControl.Type property

Obtiene el tipo del control ActiveX.

```csharp
public override ControlType Type { get; }
```

### Ejemplos

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

            // Crear botón de comando con la lista completa de parámetros
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

### Ver también

* enum [ControlType](../../controltype/)
* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


