---
title: TextBoxActiveXControl.Type
second_title: Aspose.Cells for .NET API Reference
description: TextBoxActiveXControl property. Gets the type of the ActiveX control
type: docs
url: /net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/type/
---
## TextBoxActiveXControl.Type property

Gets the type of the ActiveX control.

```csharp
public override ControlType Type { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape textBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 1, 0, 0, 200, 50);
            ActiveXControl activeXControl = textBoxShape.ActiveXControl;

            ControlType type = activeXControl.Type;
            Console.WriteLine("ActiveX Control Type: " + type);
        }
    }
}
```

### See Also

* enum [ControlType](../../controltype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


