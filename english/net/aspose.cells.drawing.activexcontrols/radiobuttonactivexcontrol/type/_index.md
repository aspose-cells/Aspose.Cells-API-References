---
title: RadioButtonActiveXControl.Type
second_title: Aspose.Cells for .NET API Reference
description: RadioButtonActiveXControl property. Gets the type of the ActiveX control
type: docs
url: /net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/type/
---
## RadioButtonActiveXControl.Type property

Gets the type of the ActiveX control.

```csharp
public override ControlType Type { get; }
```

### Examples

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class RadioButtonActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var radioShape = worksheet.Shapes.AddActiveXControl(
                ControlType.RadioButton, 
                0, // topRow
                1, // top
                0, // leftColumn
                1, // left
                100, // width
                30 // height
            );
            var activeXControl = radioShape.ActiveXControl;

            if (activeXControl.Type == ControlType.RadioButton)
            {
                RadioButtonActiveXControl radio = (RadioButtonActiveXControl)activeXControl;
                radio.Caption = "Option 1";
                radio.Value = CheckValueType.Checked;
            }

            workbook.Save("RadioButtonDemo.xlsx");
        }
    }
}
```

### See Also

* enum [ControlType](../../controltype/)
* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


