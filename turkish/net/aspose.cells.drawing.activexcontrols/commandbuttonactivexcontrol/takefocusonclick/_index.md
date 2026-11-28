---
title: "CommandButtonActiveXControl.TakeFocusOnClick"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CommandButtonActiveXControl özelliği. Denetimin tıklandığında odak alıp almayacağını gösterir"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/takefocusonclick/
---
## CommandButtonActiveXControl.TakeFocusOnClick property

Denetimin tıklandığında odak alıp almadığını gösterir.

```csharp
public bool TakeFocusOnClick { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CommandButtonActiveXControlPropertyTakeFocusOnClickDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 2, 2, 2, 2, 100, 30);
            CommandButtonActiveXControl commandButton = (CommandButtonActiveXControl)shape.ActiveXControl;

            commandButton.Caption = "Click Me";
            commandButton.TakeFocusOnClick = true;
            
            workbook.Save("CommandButtonActiveXControlTakeFocusOnClickDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


