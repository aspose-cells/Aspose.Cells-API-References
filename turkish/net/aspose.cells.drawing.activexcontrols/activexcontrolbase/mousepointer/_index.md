---
title: "ActiveXControlBase.MousePointer"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ActiveXControlBase özelliği. Kontrol için fare imleci olarak gösterilen simge tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/
---
## ActiveXControlBase.MousePointer property

Kontrol için fare imleci olarak gösterilen simge türünü alır ve ayarlar.

```csharp
public ControlMousePointerType MousePointer { get; set; }
```

### Örnekler

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

### Ayrıca Bakınız

* enum [ControlMousePointerType](../../controlmousepointertype/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


