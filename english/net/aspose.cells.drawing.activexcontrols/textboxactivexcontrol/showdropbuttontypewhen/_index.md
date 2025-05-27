---
title: TextBoxActiveXControl.ShowDropButtonTypeWhen
second_title: Aspose.Cells for .NET API Reference
description: TextBoxActiveXControl property. Specifies the symbol displayed on the drop button
type: docs
url: /net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/showdropbuttontypewhen/
---
## TextBoxActiveXControl.ShowDropButtonTypeWhen property

Specifies the symbol displayed on the drop button

```csharp
public ShowDropButtonType ShowDropButtonTypeWhen { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyShowDropButtonTypeWhenDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add an ActiveX TextBox control
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.TextBox, 
                1, 1, 1, 1, 100, 50);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;

            // Set the ShowDropButtonTypeWhen property
            textBox.ShowDropButtonTypeWhen = ShowDropButtonType.Focus;

            // Save the workbook
            workbook.Save("TextBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### See Also

* enum [ShowDropButtonType](../../showdropbuttontype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


