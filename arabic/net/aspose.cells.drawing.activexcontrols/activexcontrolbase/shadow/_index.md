---
title: "ActiveXControlBase.Shadow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ActiveXControlBase. تشير إلى ما إذا كان يجب إظهار الظل"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/
---
## ActiveXControlBase.Shadow property

يشير إلى ما إذا كان يجب إظهار الظل.

```csharp
public virtual bool Shadow { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyShadowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 2, 2, 2, 2, 100, 30);
            CommandButtonActiveXControl commandButton = (CommandButtonActiveXControl)shape.ActiveXControl;

            commandButton.Caption = "Shadow Button";
            commandButton.Shadow = true;

            workbook.Save("ActiveXControlShadowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


