---
title: "CommandButtonActiveXControl.IsWordWrapped"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CommandButtonActiveXControl. تشير إلى ما إذا كان محتوى العنصر يلتف تلقائيًا في نهاية السطر"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/iswordwrapped/
---
## CommandButtonActiveXControl.IsWordWrapped property

يشير إلى ما إذا كان محتوى العنصر يلتف تلقائيًا في نهاية السطر.

```csharp
public bool IsWordWrapped { get; set; }
```

### أمثلة

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

### انظر أيضًا

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


