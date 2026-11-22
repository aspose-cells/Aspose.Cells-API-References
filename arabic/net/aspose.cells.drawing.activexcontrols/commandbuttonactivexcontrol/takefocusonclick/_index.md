---
title: "CommandButtonActiveXControl.TakeFocusOnClick"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CommandButtonActiveXControl. تشير إلى ما إذا كان العنصر يتلقى التركيز عند النقر"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/takefocusonclick/
---
## CommandButtonActiveXControl.TakeFocusOnClick property

يشير إلى ما إذا كان التحكم يحصل على التركيز عند النقر.

```csharp
public bool TakeFocusOnClick { get; set; }
```

### أمثلة

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

### انظر أيضًا

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


