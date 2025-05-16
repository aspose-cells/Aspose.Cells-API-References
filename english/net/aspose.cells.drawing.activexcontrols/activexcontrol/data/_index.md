---
title: ActiveXControl.Data
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControl property. Gets and sets the binary data of the control
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrol/data/
---
## ActiveXControl.Data property

Gets and sets the binary data of the control.

```csharp
public override byte[] Data { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples.ActiveXControlPropertyDataDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlPropertyDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a TextBox ActiveX control with correct parameters
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 0, 0, 100, 100, 0, 0); // Added missing width and height parameters
            ActiveXControl control = shape.ActiveXControl;

            // Initialize text content
            if (control is TextBoxActiveXControl textBox)
            {
                textBox.Text = "Initial Value";
            }

            // Display initial data length
            Console.WriteLine("Initial Data Length: " + BitConverter.ToString(control.Data).Replace("-", ""));

            // Modify control properties
            if (control is TextBoxActiveXControl modifiedTextBox)
            {
                modifiedTextBox.Text = "Modified Value";
                modifiedTextBox.IsAutoSize = true;
            }

            // Display updated data length
            Console.WriteLine("Updated Data Length: " + BitConverter.ToString(control.Data).Replace("-", ""));

            workbook.Save("ActiveXControlDataDemo.xlsx");
        }
    }
}
```

### See Also

* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


