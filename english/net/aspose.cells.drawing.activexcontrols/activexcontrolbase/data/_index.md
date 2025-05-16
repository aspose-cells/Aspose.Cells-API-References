---
title: ActiveXControlBase.Data
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControlBase property. Gets and sets the binary data of the control
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrolbase/data/
---
## ActiveXControlBase.Data property

Gets and sets the binary data of the control.

```csharp
public virtual byte[] Data { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples.ActiveXControlBasePropertyDataDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace reference
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlBasePropertyDataDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a CommandButton ActiveX control
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 0, 0, 0, 0, 200, 50);
            CommandButtonActiveXControl buttonControl = (CommandButtonActiveXControl)shape.ActiveXControl;

            // Display initial Data property information
            Console.WriteLine("Initial Data length: " + buttonControl.Data.Length);

            // Modify control properties that affect Data
            buttonControl.MouseIcon = new byte[] { 0x01, 0x02, 0x03 }; // Simple mock icon data
            buttonControl.BackOleColor = 0xFF0000; // Red background

            // Display updated Data property information
            Console.WriteLine("Modified Data length: " + buttonControl.Data.Length);

            // Save the workbook to demonstrate persisted changes
            workbook.Save("ActiveXControlDataDemo.xlsx");
        }
    }
}
```

### See Also

* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


