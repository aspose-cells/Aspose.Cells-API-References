---
title: ActiveXControlBase.Workbook
second_title: Aspose.Cells for .NET API Reference
description: ActiveXControlBase property. Gets the Workbook object
type: docs
url: /net/aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/
---
## ActiveXControlBase.Workbook property

Gets the `Workbook` object.

```csharp
public Workbook Workbook { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples.ActiveXControlBasePropertyWorkbookDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlBasePropertyWorkbookDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create and add a CheckBox ActiveX control
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 0, 0, 100, 30, 0, 0);
            ActiveXControlBase control = shape.ActiveXControl;

            // Display Workbook property information
            Console.WriteLine("Control's Workbook contains " + control.Workbook.Worksheets.Count + " worksheets");

            // Modify workbook through control's Workbook reference
            control.Workbook.Worksheets[0].Cells["B2"].PutValue("Modified via ActiveXControlBase.Workbook");

            // Change other writable properties to demonstrate control manipulation
            shape.Width = 150;
            shape.Height = 40;
            shape.IsHidden = false;

            // Save modified workbook
            workbook.Save("PropertyWorkbookDemo.xlsx");
        }
    }
}
```

### See Also

* class [Workbook](../../../aspose.cells/workbook/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


