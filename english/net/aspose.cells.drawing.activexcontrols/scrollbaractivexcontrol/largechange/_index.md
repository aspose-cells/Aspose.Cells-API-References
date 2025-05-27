---
title: ScrollBarActiveXControl.LargeChange
second_title: Aspose.Cells for .NET API Reference
description: ScrollBarActiveXControl property. Gets and sets the amount by which the Position property changes
type: docs
url: /net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/largechange/
---
## ScrollBarActiveXControl.LargeChange property

Gets and sets the amount by which the Position property changes

```csharp
public int LargeChange { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ScrollBarActiveXControlPropertyLargeChangeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add a ScrollBar ActiveX Control
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 0, 1, 0, 100, 30);
            ScrollBarActiveXControl scrollBar = (ScrollBarActiveXControl)shape.ActiveXControl;

            // Set LargeChange property
            scrollBar.LargeChange = 5;

            // Save the workbook
            workbook.Save("ScrollBarActiveXControlLargeChangeDemo.xlsx");
        }
    }
}
```

### See Also

* class [ScrollBarActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


