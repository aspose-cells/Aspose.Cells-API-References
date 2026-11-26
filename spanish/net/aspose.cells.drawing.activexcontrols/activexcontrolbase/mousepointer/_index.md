---
title: "ActiveXControlBase.MousePointer"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ActiveXControlBase. Obtiene y establece el tipo de ícono que se muestra como puntero del mouse del control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/
---
## ActiveXControlBase.MousePointer property

Obtiene y establece el tipo de ícono que se muestra como puntero del mouse para el control.

```csharp
public ControlMousePointerType MousePointer { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyMousePointerDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(ControlType.CommandButton, 1, 0, 1, 0, 100, 50);
            CommandButtonActiveXControl button = (CommandButtonActiveXControl)shape.ActiveXControl;

            button.Caption = "Click Me";
            button.MousePointer = ControlMousePointerType.Help;
            button.MouseIcon = new byte[] { }; // Empty byte array for custom icon (when MousePointer is Custom)
            
            workbook.Save("ActiveXControlMousePointerDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ControlMousePointerType](../../controlmousepointertype/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


