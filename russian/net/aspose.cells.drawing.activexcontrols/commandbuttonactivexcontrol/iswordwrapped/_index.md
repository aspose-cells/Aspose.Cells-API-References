---
title: "CommandButtonActiveXControl.IsWordWrapped"
second_title: "Справочник API Aspose.Cells для .NET"
description: "CommandButtonActiveXControl property. Указывает, автоматически ли содержимое элемента управления переносится в конце строки"
type: docs
url: /ru/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/iswordwrapped/
---
## CommandButtonActiveXControl.IsWordWrapped property

Указывает, будет ли содержимое контрола автоматически переноситься в конце строки.

```csharp
public bool IsWordWrapped { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CommandButtonActiveXControlPropertyIsWordWrappedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 0, 0, 2, 2, 150, 30);
            CommandButtonActiveXControl button = (CommandButtonActiveXControl)shape.ActiveXControl;

            button.Caption = "Click to demonstrate word wrapping in caption";
            button.IsWordWrapped = true;

            workbook.Save("CommandButtonIsWordWrappedDemo.xlsm");
        }
    }
}
```

### См. также

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


